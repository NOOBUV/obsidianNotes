#### Findings
There was a change in timestamp that was being recorded for the day. It shifted 1 hour early from 12:30 to 11:30 hence in frontend it was recording 23h instead of 24 that's why graphs were not visible.

#### Reason
Due to US-daylight saving issue the timestamp got shifted