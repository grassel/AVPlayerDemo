
### AVPlayerDemo ###

===========================================================================
DESCRIPTION:

Uses AVPlayer to play videos from the iPod Library, Camera Roll, or via iTunes File Sharing. Also displays metadata information for the video.

===========================================================================
BUILD REQUIREMENTS:

iOS 7.0 SDK or later

===========================================================================
RUNTIME REQUIREMENTS:

iOS 7.0 or later

===========================================================================
USING THE SAMPLE:

The sample will list all videos in the iPod Library, Camera Roll or those available via iTunes File Sharing. Navigate to each of these different lists with the tab bar icons. Select a video from any of these lists and a playback window will be brought up complete with a movie controller. Touch the play control and the video will begin playing. Tap the info. icon to view metadata for the video.

===========================================================================
NOTES:

As discussed in "Enhancements for HTTP Live Streaming" in the AV Foundation Release Notes for iOS 4.3, the inspection features of AVURLAsset have been enhanced to handle HTTP Live Streaming Media resources. For this reason, starting with iOS 4.3 you can prepare any asset for playback in a uniform way, according to the best practices originally outlined for file-based assets in the AV Foundation Programming Guide. Those steps are as follows:



3. Associate the item with an instance of AVPlayer. 

4. Wait until the item�s status indicates that it�s ready to play.



Duration of Timed Media Resources for Playback



CMTime itemDuration = kCMTimeInvalid;

if ([AVPlayerItem instancesRespondToSelector:@selector (duration)]) 
{
{

===========================================================================
CHANGES FROM PREVIOUS VERSIONS:

1.2 - Fixed problem where the metadata screen would not dismiss properly. Fixed deprecated call warnings. Other miscellaneous changes.

1.1 - Update for iOS 4.3 to show how to prepare any asset for playback in a uniform way, plus new technique for obtaining duration of a AVPlayerItem.

1.0 - First Release

===========================================================================
Copyright (C) 2010-2014 Apple Inc. All rights reserved.