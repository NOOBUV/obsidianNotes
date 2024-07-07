First checked whether the call we got is using bform or tform using a boolean.

Findings about updateImage:
first it was checking whether the media object already had url generated for it
If it wasn't then we were generating the url

Changes i made in updateImage:
if media object was present then checked whether this it has generated typeform url or not if it doesn't then we were checking is this bform then fetching the image from s3 url
if media object was not present then we were checking boolean true for typeform compatible = true if it was typeform else false
now we were sending this typeform compatible boolean with request to backend where if typeform_compatible was true then backend was generating url for typeform else it wasn't and we were assigning href links according to type of form. 
