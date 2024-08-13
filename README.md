# oz-YouTube-Downloader-

This program is a multifunctional tool called oz YouTube Downloader, designed for downloading YouTube videos and playlists, with support for user-customizable download settings. The main features of the program include:

1.Download Video and Audio: Users can input a YouTube video or playlist URL, choose the download format (mp3 or mp4), and the program will automatically download the specified content.

2.Playlist Support: It can handle YouTube playlists, downloading each video one by one, even continuing to download other videos if some fail.

3.User Preferences: Users can customize the output directory, audio quality, and video quality, with these settings saved in a preferences.json file. The program loads these preferences at startup.

4.Multilingual Support: Upon the first launch, users can select a language (currently supporting English, Simplified Chinese, Spanish, Russian, French, and Traditional Chinese), and can change the language anytime in the settings.

5.Logging: The program generates a log file at startup to record operations and error messages. The log file is saved in the log directory, and when the total log file size exceeds 5MB, old log files will be automatically deleted.

6.Program Integrity Check: At startup, it checks if FFmpeg is installed and verifies network connection status. If issues are detected, it prompts the user to resolve them.

7.GitHub Update Check: At startup, it checks for new versions available on GitHub, and if a new version is found, it prompts the user to download the update.

Usage Steps:

1.First Launch: The program will ask the user to select a language. After selection, it will generate a preferences.json file and save the default settings along with the user's language choice.

2.Download Operation:

Input a YouTube video or playlist URL, or input the path to a .txt file containing multiple URLs.
Choose the download format (1 for mp3, 2 for mp4).
The program will start downloading and display the number of successful and failed downloads, with the URLs of failed videos shown to the user.
Modify User Preferences: Users can change the output directory, audio quality, video quality, or language settings through menu options.

# Installation

<a href="https://github.com/oz2011/oz-YouTube-Downloader-/releases">
  <img src="https://github.com/machiav3lli/oandbackupx/raw/034b226cea5c1b30eb4f6a6f313e4dadcbb0ece4/badge_github.png" alt="GET IT" width="300"/>
</a>


# Disclaimer
This project and its contents are not affiliated with, funded, authorized, endorsed by, or in any way associated with YouTube, Google LLC or any of its affiliates and subsidiaries.

Any trademark, service mark, trade name, or other intellectual property rights used in this project are owned by the respective owners.

# License
`© 2024, oz (fisherw0311@gmail.com)`

Licensed under the GNU General Public License, Version 3.0 (the "License"); You may not use this file except in compliance with the License. You may obtain a copy of the License at

http://www.gnu.org/licenses/#GPL

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.
