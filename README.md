# mpScoreCard
MountainProjectScoreCard is a tampermonkey script which adds 8a.nu type scores to users on mountainproject.com

This is my version of the scorecard. I made some minor changes to the orginal version at: https://github.com/aawait1234/mpScoreCard

# Installation
See https://docs.google.com/document/d/1vMzY-NWaR75HM9YFOHCdOa1WXts_U0Dn-wg59kA6WB4/edit?usp=sharing

# Scoring
* Looks at last 5 pages of ticks
* Takes top ten scores
* Base points for routes:
  * 10a and below, 0 points
  * 10b 0.75 points
  * 10c 1.5 points
  * 10d 2.25 points
  * 11a 3 points
  * and so on
* Base points for boulders:
  * V0 0 points
  * V1 1 point
  * V2 2 points
  * and so on
* Bonus points
  * 1 point for flash
  * 1.5 points for onsight
  * 1.5 points for trad routes

# Changes to Aaron's script
* Base score of zero for 10a and below, follow Aaron's equation for 10b and above.
* No points for just attempting the route.
* Add 1.5 points for trad route.
* Keep slash grades for routes (but not boulders) and give the average of the two letters.
* Convert plus/minus/ or just '5.10', for example, to slash grades.
  * Fixes bug with these type of routes where 5.10 would be ignored and 5.10+ wouldn't give any more points than 10a.
* Did not change the behavior for slash grades or plus/minus grades on boulders.
* Go back through 5 pages of ticks instead of 3.
* Removed the stipulation that climbs must be in this calendar year.
* Scores the top ten climbs instead of the top five.
* Modified "isSend" to remove the climb if note includes Follow or TR or Hung.


