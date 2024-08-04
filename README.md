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

Code Structure:
main(): The main entry point of the program, responsible for initializing logging, loading user preferences, checking program integrity and network connection, checking for GitHub updates, and providing a user operation menu.

setup_logging(): Sets up logging and manages log file sizes.

check_ffmpeg() and check_network(): Check the installation status of FFmpeg and the network connection status.

check_github_release(): Checks for the latest version on GitHub.

load_preferences() and save_preferences(): Load and save user preferences.

reset_preferences(): Resets user preferences to default values.

load_language_file(): Loads the language file.

download_youtube_media(): Downloads YouTube videos or playlists.

set_preferences(): Provides options for users to modify their preferences.
