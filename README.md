# API Random Twitch Clip
 
# Description
Utility that retrieves 100 Twitch clips and randomly picks one. Date filter included for the past 12 months (configurable). Add this to a play effect, chat message, etc.

# Requirement
- Firebot 5.57.0-nightly-23.03.22 (JSON Stringify is bugged in 5.57.0)

# Install
+ Download API Random Twitch Clip.firebotsetup
+ Import the downloaded file
  + Preset Effect List will be named [API] Get User Clips

# Usage and Variables
+ Date filter
  + Custom Variable: PreviousYear
    + Calculated from today
  + Custom Variable: CurrentDate
  + To disable date filter
    + Disable the HTTP Request effect labeled (Date Filter)
    + Enable the HTTP Request effect labeled (No Date Filter)
+ Twitch clips variables
  + twitchClipsJson: Retrieved list of Twitch clips
  + twitchClipsData: Randomized array of Twitch clips
    + Use index zero for playing the clip and pulling other elements out for display purposes, refer to Twitch API documentation for fields
+ Clip title
  + Custom Variable: ClipTitle
    + Checks the length of the clip title and truncates it at 60 characters
+ Clip date
  + Custom Variable: ClipDate
    + Used for displaying the date of the clip, currently formatted as YYYY-MM-DD

# References
+ https://dev.twitch.tv/docs/api/videos/

# Credits
+ Raimen (coding hints)
