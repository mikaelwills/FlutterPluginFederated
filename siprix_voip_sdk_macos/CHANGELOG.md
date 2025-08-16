## 1.0.11
- Fixed crash on ios/macos when license string is empty
- Added fix which prevents long delay on collecting candidates when enabled STUN
- Added handler for case when connection can't be created because of wrong STUN/TURN address
- Added new option 'ini.transpForceIPv4'
  //2025.08.16

## 1.0.10
- Prevent potential crash on hold when call initiated as video/fixed handling Hold events
- Fixed bug which prevents adding multiple TLS transports
- Fixed TURN address resolution
- 'OnMessageIncoming' API update (added messageId arg)
  //2025.08.09

## 1.0.9
- Added new account properties 'stunServer','turnServer'
- Added new ini property 'VideoCallEnabled'
- Added new video data property 'Rotation'
- Fixed handling ACK/SDP response (missed 'onCallConnected' event)
- Fixed potential crash when received SIP MESSAGE without body
  //2025.07.31

## 1.0.8
- Added new method 'stopRingtone'
  //2025.06.04

## 1.0.7
- Fixed bug with find local account which matches received SIP request
- Added new option 'iceEnabled'

## 1.0.6
- Improved CallRecording (capture local+remote sound, use mp3 encoder, write mono or stereo)
- Added new ini properties 'recordStereo', 'useDnsSrv'

## 1.0.5
- Fixed bug with sending statusCode in the 'onTerminated' callback
- Added ability to switch calls automatically after call un-held, connected

## 1.0.4
- Added new ini property 'UnregOnDestroy'

## 1.0.3
- Added ability to send and receive text messages (SIP MESSAGE request)
- Added ability to override DisplayName in outgoing call (method 'Dest_SetDisplayName')
- Added ability to handle received MediaControlEvent 'picture_fast_update'
- Fixed bug in 'RewriteContactIp' option implementation when TCP/TLS transport is using
- Fixed parsing RTCP FB parameters of video in SDP

## 1.0.2 * 
* Fixed handling case when app adds duplicate subscription.
* Now library raises error 'ESubscrAlreadyExist' and also returns existing subscrId

## 1.0.1
* Fixed podspec file for ios/macos
* Added new ini property 'brandName'
* Enabled ability to make attended transfer when call on hold

## 1.0.0
* Initial release. 
* Contains implementation based on method channels.
