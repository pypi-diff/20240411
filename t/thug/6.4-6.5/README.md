# Comparing `tmp/thug-6.4.tar.gz` & `tmp/thug-6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thug-6.4.tar", last modified: Thu Apr  4 17:17:07 2024, max compression
+gzip compressed data, was "thug-6.5.tar", last modified: Thu Apr 11 14:03:15 2024, max compression
```

## Comparing `thug-6.4.tar` & `thug-6.5.tar`

### file list

```diff
@@ -1,520 +1,555 @@
-drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.693176 thug-6.4/
--rw-r--r--   0 buffer     (501) staff       (20)    17987 2024-03-21 15:01:28.000000 thug-6.4/LICENSE.txt
--rw-r--r--   0 buffer     (501) staff       (20)      130 2024-03-21 15:01:28.000000 thug-6.4/MANIFEST.in
--rw-r--r--   0 buffer     (501) staff       (20)     5535 2024-04-04 17:17:07.692989 thug-6.4/PKG-INFO
--rw-r--r--   0 buffer     (501) staff       (20)     2695 2024-03-21 15:01:28.000000 thug-6.4/README.rst
--rw-r--r--   0 buffer     (501) staff       (20)     3765 2024-04-03 20:13:22.000000 thug-6.4/pyproject.toml
--rw-r--r--   0 buffer     (501) staff       (20)       38 2024-04-04 17:17:07.693216 thug-6.4/setup.cfg
-drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.629256 thug-6.4/thug/
-drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.631259 thug-6.4/thug/ActiveX/
--rw-r--r--   0 buffer     (501) staff       (20)     7458 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/ActiveX.py
--rw-r--r--   0 buffer     (501) staff       (20)    46031 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/CLSID.py
--rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/__init__.py
-drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.647273 thug-6.4/thug/ActiveX/modules/
--rw-r--r--   0 buffer     (501) staff       (20)      323 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/AOLAttack.py
--rw-r--r--   0 buffer     (501) staff       (20)      871 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/AcroPDF.py
--rw-r--r--   0 buffer     (501) staff       (20)      610 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/AdodbRecordset.py
--rw-r--r--   0 buffer     (501) staff       (20)     2404 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/AdodbStream.py
--rw-r--r--   0 buffer     (501) staff       (20)     1275 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/AnswerWorks.py
--rw-r--r--   0 buffer     (501) staff       (20)      948 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/AolAmpX.py
--rw-r--r--   0 buffer     (501) staff       (20)      736 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/AolICQ.py
--rw-r--r--   0 buffer     (501) staff       (20)      620 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/BaiduBar.py
--rw-r--r--   0 buffer     (501) staff       (20)      498 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/BitDefender.py
--rw-r--r--   0 buffer     (501) staff       (20)      360 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/CABrightStor.py
--rw-r--r--   0 buffer     (501) staff       (20)      531 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/CGAgent.py
--rw-r--r--   0 buffer     (501) staff       (20)      446 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/Comodo.py
--rw-r--r--   0 buffer     (501) staff       (20)      652 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/ConnectAndEnterRoom.py
--rw-r--r--   0 buffer     (501) staff       (20)      245 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/CreativeSoftAttack.py
--rw-r--r--   0 buffer     (501) staff       (20)      408 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/DLinkMPEG.py
--rw-r--r--   0 buffer     (501) staff       (20)      605 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/DPClient.py
--rw-r--r--   0 buffer     (501) staff       (20)      411 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/DVRHOSTWeb.py
--rw-r--r--   0 buffer     (501) staff       (20)      548 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/DirectShow.py
--rw-r--r--   0 buffer     (501) staff       (20)      342 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/DivX.py
--rw-r--r--   0 buffer     (501) staff       (20)     1651 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/Domino.py
--rw-r--r--   0 buffer     (501) staff       (20)     1170 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/EnjoySAP.py
--rw-r--r--   0 buffer     (501) staff       (20)      751 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/FacebookPhotoUploader.py
--rw-r--r--   0 buffer     (501) staff       (20)     3094 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/File.py
--rw-r--r--   0 buffer     (501) staff       (20)      441 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/FileUploader.py
--rw-r--r--   0 buffer     (501) staff       (20)     2252 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/Folder.py
--rw-r--r--   0 buffer     (501) staff       (20)      460 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/GLIEDown2.py
--rw-r--r--   0 buffer     (501) staff       (20)      677 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/GatewayWeblaunch.py
--rw-r--r--   0 buffer     (501) staff       (20)      383 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/Gogago.py
--rw-r--r--   0 buffer     (501) staff       (20)      492 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/GomWeb.py
--rw-r--r--   0 buffer     (501) staff       (20)     2728 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/HPInfo.py
--rw-r--r--   0 buffer     (501) staff       (20)      407 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/ICQToolbar.py
--rw-r--r--   0 buffer     (501) staff       (20)      807 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/IMWebControl.py
--rw-r--r--   0 buffer     (501) staff       (20)      413 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/InternetCleverSuite.py
--rw-r--r--   0 buffer     (501) staff       (20)     1750 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/JavaDeploymentToolkit.py
--rw-r--r--   0 buffer     (501) staff       (20)      932 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/JetAudioDownloadFromMusicStore.py
--rw-r--r--   0 buffer     (501) staff       (20)      368 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/Kingsoft.py
--rw-r--r--   0 buffer     (501) staff       (20)      652 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/MSRICHTXT.py
--rw-r--r--   0 buffer     (501) staff       (20)      411 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/MSVFP.py
--rw-r--r--   0 buffer     (501) staff       (20)      457 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/MSXML2DOMDocument.py
--rw-r--r--   0 buffer     (501) staff       (20)     3549 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/MacrovisionFlexNet.py
--rw-r--r--   0 buffer     (501) staff       (20)      295 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/MicrosoftWorks7Attack.py
--rw-r--r--   0 buffer     (501) staff       (20)     2119 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/MicrosoftXMLDOM.py
--rw-r--r--   0 buffer     (501) staff       (20)     7787 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/MicrosoftXMLHTTP.py
--rw-r--r--   0 buffer     (501) staff       (20)      430 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/Move.py
--rw-r--r--   0 buffer     (501) staff       (20)      376 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/MyspaceUploader.py
--rw-r--r--   0 buffer     (501) staff       (20)      520 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/NCTAudioFile2.py
--rw-r--r--   0 buffer     (501) staff       (20)      972 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/NamoInstaller.py
--rw-r--r--   0 buffer     (501) staff       (20)      547 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/NeoTracePro.py
--rw-r--r--   0 buffer     (501) staff       (20)     2210 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/NessusScanCtrl.py
--rw-r--r--   0 buffer     (501) staff       (20)      945 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/OfficeOCX.py
--rw-r--r--   0 buffer     (501) staff       (20)      919 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/OurgameGLWorld.py
--rw-r--r--   0 buffer     (501) staff       (20)     1066 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/PPlayer.py
--rw-r--r--   0 buffer     (501) staff       (20)      462 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/PTZCamPanel.py
--rw-r--r--   0 buffer     (501) staff       (20)      458 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/QuantumStreaming.py
--rw-r--r--   0 buffer     (501) staff       (20)      447 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/QvodCtrl.py
--rw-r--r--   0 buffer     (501) staff       (20)      712 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/RDSDataSpace.py
--rw-r--r--   0 buffer     (501) staff       (20)     2063 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/RealPlayer.py
--rw-r--r--   0 buffer     (501) staff       (20)      285 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/RediffBolDownloaderAttack.py
--rw-r--r--   0 buffer     (501) staff       (20)      684 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/RegistryPro.py
--rw-r--r--   0 buffer     (501) staff       (20)      316 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/RisingScanner.py
--rw-r--r--   0 buffer     (501) staff       (20)      412 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/RtspVaPgCtrl.py
--rw-r--r--   0 buffer     (501) staff       (20)      980 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/SSReaderPdg2.py
--rw-r--r--   0 buffer     (501) staff       (20)     1032 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/ScriptingDictionary.py
--rw-r--r--   0 buffer     (501) staff       (20)      342 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/ScriptingEncoder.py
--rw-r--r--   0 buffer     (501) staff       (20)     4975 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/ScriptingFileSystemObject.py
--rw-r--r--   0 buffer     (501) staff       (20)     1184 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/ShellApplication.py
--rw-r--r--   0 buffer     (501) staff       (20)      298 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/Shockwave.py
--rw-r--r--   0 buffer     (501) staff       (20)      390 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/ShockwaveFlash10.py
--rw-r--r--   0 buffer     (501) staff       (20)      390 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/ShockwaveFlash11.py
--rw-r--r--   0 buffer     (501) staff       (20)      390 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/ShockwaveFlash12.py
--rw-r--r--   0 buffer     (501) staff       (20)      390 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/ShockwaveFlash9.py
--rw-r--r--   0 buffer     (501) staff       (20)      274 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/SilverLight.py
--rw-r--r--   0 buffer     (501) staff       (20)      752 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/SinaDLoader.py
--rw-r--r--   0 buffer     (501) staff       (20)     1165 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/SnapshotViewer.py
--rw-r--r--   0 buffer     (501) staff       (20)      646 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/SonicWallNetExtenderAddRouteEntry.py
--rw-r--r--   0 buffer     (501) staff       (20)      754 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/Spreadsheet.py
--rw-r--r--   0 buffer     (501) staff       (20)      609 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/StormConfig.py
--rw-r--r--   0 buffer     (501) staff       (20)     2028 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/StormMps.py
--rw-r--r--   0 buffer     (501) staff       (20)      480 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/StreamAudioChainCast.py
--rw-r--r--   0 buffer     (501) staff       (20)      854 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/SymantecAppStream.py
--rw-r--r--   0 buffer     (501) staff       (20)     1949 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/SymantecBackupExec.py
--rw-r--r--   0 buffer     (501) staff       (20)     4792 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/TextStream.py
--rw-r--r--   0 buffer     (501) staff       (20)      713 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/Toshiba.py
--rw-r--r--   0 buffer     (501) staff       (20)      330 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/UUSeeUpdate.py
--rw-r--r--   0 buffer     (501) staff       (20)      502 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/UniversalUpload.py
--rw-r--r--   0 buffer     (501) staff       (20)     1445 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/VLC.py
--rw-r--r--   0 buffer     (501) staff       (20)      527 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/VisualStudioDTE80.py
--rw-r--r--   0 buffer     (501) staff       (20)      493 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/VsaIDEDTE.py
--rw-r--r--   0 buffer     (501) staff       (20)      493 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/VsmIDEDTE.py
--rw-r--r--   0 buffer     (501) staff       (20)      815 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/WMEncProfileManager.py
--rw-r--r--   0 buffer     (501) staff       (20)      132 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/WMP.py
--rw-r--r--   0 buffer     (501) staff       (20)      257 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/WScriptCollection.py
--rw-r--r--   0 buffer     (501) staff       (20)     1279 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/WScriptExec.py
--rw-r--r--   0 buffer     (501) staff       (20)     1726 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/WScriptNetwork.py
--rw-r--r--   0 buffer     (501) staff       (20)     8198 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/WScriptShell.py
--rw-r--r--   0 buffer     (501) staff       (20)      218 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/WScriptShortcut.py
--rw-r--r--   0 buffer     (501) staff       (20)      590 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/WebViewFolderIcon.py
--rw-r--r--   0 buffer     (501) staff       (20)     1358 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/WinNTSystemInfo.py
--rw-r--r--   0 buffer     (501) staff       (20)      530 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/WinZip.py
--rw-r--r--   0 buffer     (501) staff       (20)      145 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/WindowsMediaPlayer.py
--rw-r--r--   0 buffer     (501) staff       (20)      921 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/XMLDOMParseError.py
--rw-r--r--   0 buffer     (501) staff       (20)      888 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/XUpload.py
--rw-r--r--   0 buffer     (501) staff       (20)      976 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/YahooJukebox.py
--rw-r--r--   0 buffer     (501) staff       (20)      446 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/YahooMessengerCyft.py
--rw-r--r--   0 buffer     (501) staff       (20)      939 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/YahooMessengerYVerInfo.py
--rw-r--r--   0 buffer     (501) staff       (20)     1102 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/YahooMessengerYwcvwr.py
--rw-r--r--   0 buffer     (501) staff       (20)     1660 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/ZenturiProgramCheckerAttack.py
--rw-r--r--   0 buffer     (501) staff       (20)     2079 2024-03-21 15:01:28.000000 thug-6.4/thug/ActiveX/modules/__init__.py
-drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.647395 thug-6.4/thug/Analysis/
--rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/Analysis/__init__.py
-drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.647600 thug-6.4/thug/Analysis/awis/
--rw-r--r--   0 buffer     (501) staff       (20)     3488 2024-03-21 15:01:28.000000 thug-6.4/thug/Analysis/awis/AWIS.py
--rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/Analysis/awis/__init__.py
-drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.647798 thug-6.4/thug/Analysis/context/
--rw-r--r--   0 buffer     (501) staff       (20)     1609 2024-03-21 15:01:28.000000 thug-6.4/thug/Analysis/context/ContextAnalyzer.py
--rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/Analysis/context/__init__.py
-drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.647995 thug-6.4/thug/Analysis/favicon/
--rw-r--r--   0 buffer     (501) staff       (20)      394 2024-03-21 15:01:28.000000 thug-6.4/thug/Analysis/favicon/Favicon.py
--rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/Analysis/favicon/__init__.py
-drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.648198 thug-6.4/thug/Analysis/honeyagent/
--rw-r--r--   0 buffer     (501) staff       (20)     3980 2024-03-21 15:01:28.000000 thug-6.4/thug/Analysis/honeyagent/HoneyAgent.py
--rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/Analysis/honeyagent/__init__.py
-drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.648432 thug-6.4/thug/Analysis/screenshot/
--rw-r--r--   0 buffer     (501) staff       (20)     1309 2024-03-21 15:01:28.000000 thug-6.4/thug/Analysis/screenshot/Screenshot.py
--rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/Analysis/screenshot/__init__.py
-drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.648717 thug-6.4/thug/Analysis/shellcode/
--rw-r--r--   0 buffer     (501) staff       (20)     8118 2024-03-21 15:01:28.000000 thug-6.4/thug/Analysis/shellcode/Shellcode.py
--rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/Analysis/shellcode/__init__.py
-drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.649960 thug-6.4/thug/Classifier/
--rw-r--r--   0 buffer     (501) staff       (20)     5394 2024-03-21 15:01:28.000000 thug-6.4/thug/Classifier/BaseClassifier.py
--rw-r--r--   0 buffer     (501) staff       (20)     2094 2024-03-21 15:01:28.000000 thug-6.4/thug/Classifier/CookieClassifier.py
--rw-r--r--   0 buffer     (501) staff       (20)     2147 2024-03-21 15:01:28.000000 thug-6.4/thug/Classifier/HTMLClassifier.py
--rw-r--r--   0 buffer     (501) staff       (20)     2057 2024-03-21 15:01:28.000000 thug-6.4/thug/Classifier/ImageClassifier.py
--rw-r--r--   0 buffer     (501) staff       (20)     1996 2024-03-21 15:01:28.000000 thug-6.4/thug/Classifier/JSClassifier.py
--rw-r--r--   0 buffer     (501) staff       (20)     2230 2024-03-21 15:01:28.000000 thug-6.4/thug/Classifier/SampleClassifier.py
--rw-r--r--   0 buffer     (501) staff       (20)     2070 2024-03-21 15:01:28.000000 thug-6.4/thug/Classifier/TextClassifier.py
--rw-r--r--   0 buffer     (501) staff       (20)     2318 2024-03-21 15:01:28.000000 thug-6.4/thug/Classifier/URLClassifier.py
--rw-r--r--   0 buffer     (501) staff       (20)     2002 2024-03-21 15:01:28.000000 thug-6.4/thug/Classifier/VBSClassifier.py
--rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/Classifier/__init__.py
-drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.657016 thug-6.4/thug/DOM/
--rw-r--r--   0 buffer     (501) staff       (20)     2327 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/Alexa.py
--rw-r--r--   0 buffer     (501) staff       (20)     2236 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/AsyncPrefetcher.py
--rw-r--r--   0 buffer     (501) staff       (20)     2298 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/CCInterpreter.py
--rw-r--r--   0 buffer     (501) staff       (20)      878 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/Chrome.py
--rw-r--r--   0 buffer     (501) staff       (20)     1302 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/ClipboardData.py
--rw-r--r--   0 buffer     (501) staff       (20)      817 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/Components.py
--rw-r--r--   0 buffer     (501) staff       (20)     5685 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/Console.py
--rw-r--r--   0 buffer     (501) staff       (20)     1113 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/Crypto.py
--rw-r--r--   0 buffer     (501) staff       (20)    56116 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/DFT.py
--rw-r--r--   0 buffer     (501) staff       (20)     3511 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/External.py
--rw-r--r--   0 buffer     (501) staff       (20)     2831 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/HTMLInspector.py
--rw-r--r--   0 buffer     (501) staff       (20)    10997 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/HTTPSession.py
--rw-r--r--   0 buffer     (501) staff       (20)      932 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/HTTPSessionException.py
--rw-r--r--   0 buffer     (501) staff       (20)     3717 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/History.py
--rw-r--r--   0 buffer     (501) staff       (20)     3501 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/JSClass.py
--rw-r--r--   0 buffer     (501) staff       (20)     8294 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/JSEngine.py
--rw-r--r--   0 buffer     (501) staff       (20)     4395 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/JSInspector.py
--rw-r--r--   0 buffer     (501) staff       (20)     5971 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/JScriptEncode.py
--rw-r--r--   0 buffer     (501) staff       (20)      752 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/LocalStorage.py
--rw-r--r--   0 buffer     (501) staff       (20)     4873 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/Location.py
--rw-r--r--   0 buffer     (501) staff       (20)    18649 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/MIMEHandler.py
--rw-r--r--   0 buffer     (501) staff       (20)      762 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/Map.py
--rw-r--r--   0 buffer     (501) staff       (20)     1195 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/MimeType.py
--rw-r--r--   0 buffer     (501) staff       (20)     4504 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/MimeTypes.py
--rw-r--r--   0 buffer     (501) staff       (20)      782 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/MozConnection.py
--rw-r--r--   0 buffer     (501) staff       (20)    13892 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/Navigator.py
--rw-r--r--   0 buffer     (501) staff       (20)     4191 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/Personality.py
--rw-r--r--   0 buffer     (501) staff       (20)     1231 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/Plugin.py
--rw-r--r--   0 buffer     (501) staff       (20)     1469 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/Plugins.py
--rw-r--r--   0 buffer     (501) staff       (20)     1064 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/SchemeHandler.py
--rw-r--r--   0 buffer     (501) staff       (20)     5954 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/Screen.py
--rw-r--r--   0 buffer     (501) staff       (20)      756 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/SessionStorage.py
--rw-r--r--   0 buffer     (501) staff       (20)     1775 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/Sidebar.py
--rw-r--r--   0 buffer     (501) staff       (20)     2830 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/Storage.py
--rw-r--r--   0 buffer     (501) staff       (20)     2805 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/UserProfile.py
--rw-r--r--   0 buffer     (501) staff       (20)      766 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/Utils.py
-drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.657648 thug-6.4/thug/DOM/W3C/
-drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.660670 thug-6.4/thug/DOM/W3C/Core/
--rw-r--r--   0 buffer     (501) staff       (20)     2172 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Core/Attr.py
--rw-r--r--   0 buffer     (501) staff       (20)      266 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Core/CDATASection.py
--rw-r--r--   0 buffer     (501) staff       (20)     1245 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Core/CharacterData.py
--rw-r--r--   0 buffer     (501) staff       (20)     3760 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Core/ClassList.py
--rw-r--r--   0 buffer     (501) staff       (20)      565 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Core/Comment.py
--rw-r--r--   0 buffer     (501) staff       (20)     1893 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Core/DOMException.py
--rw-r--r--   0 buffer     (501) staff       (20)     4988 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Core/DOMImplementation.py
--rw-r--r--   0 buffer     (501) staff       (20)     8842 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Core/Document.py
--rw-r--r--   0 buffer     (501) staff       (20)     2422 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Core/DocumentFragment.py
--rw-r--r--   0 buffer     (501) staff       (20)     1512 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Core/DocumentType.py
--rw-r--r--   0 buffer     (501) staff       (20)     9703 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Core/Element.py
--rw-r--r--   0 buffer     (501) staff       (20)      458 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Core/Entity.py
--rw-r--r--   0 buffer     (501) staff       (20)      501 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Core/EntityReference.py
--rw-r--r--   0 buffer     (501) staff       (20)     1295 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Core/NamedNodeMap.py
--rw-r--r--   0 buffer     (501) staff       (20)    14383 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Core/Node.py
--rw-r--r--   0 buffer     (501) staff       (20)      617 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Core/NodeList.py
--rw-r--r--   0 buffer     (501) staff       (20)      341 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Core/NodeType.py
--rw-r--r--   0 buffer     (501) staff       (20)      486 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Core/Notation.py
--rw-r--r--   0 buffer     (501) staff       (20)      507 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Core/ProcessingInstruction.py
--rw-r--r--   0 buffer     (501) staff       (20)      804 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Core/Text.py
--rw-r--r--   0 buffer     (501) staff       (20)      939 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Core/__init__.py
--rw-r--r--   0 buffer     (501) staff       (20)      362 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Core/abstractmethod.py
--rw-r--r--   0 buffer     (501) staff       (20)      274 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/DOMParser.py
--rw-r--r--   0 buffer     (501) staff       (20)     1453 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/DOMTokenList.py
-drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.662004 thug-6.4/thug/DOM/W3C/Events/
--rw-r--r--   0 buffer     (501) staff       (20)      828 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Events/DocumentEvent.py
--rw-r--r--   0 buffer     (501) staff       (20)     4094 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Events/Event.py
--rw-r--r--   0 buffer     (501) staff       (20)      477 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Events/EventException.py
--rw-r--r--   0 buffer     (501) staff       (20)      274 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Events/EventListener.py
--rw-r--r--   0 buffer     (501) staff       (20)     9365 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Events/EventTarget.py
--rw-r--r--   0 buffer     (501) staff       (20)      389 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Events/HTMLEvent.py
--rw-r--r--   0 buffer     (501) staff       (20)     1174 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Events/MessageEvent.py
--rw-r--r--   0 buffer     (501) staff       (20)     2068 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Events/MouseEvent.py
--rw-r--r--   0 buffer     (501) staff       (20)     1557 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Events/MutationEvent.py
--rw-r--r--   0 buffer     (501) staff       (20)     1113 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Events/StorageEvent.py
--rw-r--r--   0 buffer     (501) staff       (20)      634 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Events/UIEvent.py
--rw-r--r--   0 buffer     (501) staff       (20)      628 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Events/__init__.py
-drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.662329 thug-6.4/thug/DOM/W3C/File/
--rw-r--r--   0 buffer     (501) staff       (20)     2380 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/File/Blob.py
--rw-r--r--   0 buffer     (501) staff       (20)     1377 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/File/File.py
--rw-r--r--   0 buffer     (501) staff       (20)       74 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/File/__init__.py
-drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.673074 thug-6.4/thug/DOM/W3C/HTML/
--rw-r--r--   0 buffer     (501) staff       (20)      194 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/AudioTrackList.py
--rw-r--r--   0 buffer     (501) staff       (20)      611 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/Dataset.py
--rw-r--r--   0 buffer     (501) staff       (20)      374 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLAllCollection.py
--rw-r--r--   0 buffer     (501) staff       (20)     1878 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLAnchorElement.py
--rw-r--r--   0 buffer     (501) staff       (20)      626 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLAppletElement.py
--rw-r--r--   0 buffer     (501) staff       (20)      247 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLAudioElement.py
--rw-r--r--   0 buffer     (501) staff       (20)      252 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLBRElement.py
--rw-r--r--   0 buffer     (501) staff       (20)      289 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLBaseElement.py
--rw-r--r--   0 buffer     (501) staff       (20)      329 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLBaseFontElement.py
--rw-r--r--   0 buffer     (501) staff       (20)     1484 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLBodyElement.py
--rw-r--r--   0 buffer     (501) staff       (20)      561 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLButtonElement.py
--rw-r--r--   0 buffer     (501) staff       (20)     1278 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLCollection.py
--rw-r--r--   0 buffer     (501) staff       (20)      265 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLDListElement.py
--rw-r--r--   0 buffer     (501) staff       (20)      263 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLDirectoryElement.py
--rw-r--r--   0 buffer     (501) staff       (20)      253 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLDivElement.py
--rw-r--r--   0 buffer     (501) staff       (20)    16355 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLDocument.py
--rw-r--r--   0 buffer     (501) staff       (20)      952 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLDocumentCompatibleInfo.py
--rw-r--r--   0 buffer     (501) staff       (20)      412 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLDocumentCompatibleInfoCollection.py
--rw-r--r--   0 buffer     (501) staff       (20)     4438 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLElement.py
--rw-r--r--   0 buffer     (501) staff       (20)      332 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLFieldSetElement.py
--rw-r--r--   0 buffer     (501) staff       (20)      320 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLFontElement.py
--rw-r--r--   0 buffer     (501) staff       (20)      204 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLFormControlsCollection.py
--rw-r--r--   0 buffer     (501) staff       (20)     1689 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLFormElement.py
--rw-r--r--   0 buffer     (501) staff       (20)      948 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLFrameElement.py
--rw-r--r--   0 buffer     (501) staff       (20)      289 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLFrameSetElement.py
--rw-r--r--   0 buffer     (501) staff       (20)      400 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLHRElement.py
--rw-r--r--   0 buffer     (501) staff       (20)      258 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLHeadElement.py
--rw-r--r--   0 buffer     (501) staff       (20)      257 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLHeadingElement.py
--rw-r--r--   0 buffer     (501) staff       (20)      258 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLHtmlElement.py
--rw-r--r--   0 buffer     (501) staff       (20)     1219 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLIFrameElement.py
--rw-r--r--   0 buffer     (501) staff       (20)     1233 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLImageElement.py
--rw-r--r--   0 buffer     (501) staff       (20)     1330 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLInputElement.py
--rw-r--r--   0 buffer     (501) staff       (20)      275 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLIsIndexElement.py
--rw-r--r--   0 buffer     (501) staff       (20)      290 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLLIElement.py
--rw-r--r--   0 buffer     (501) staff       (20)      366 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLLabelElement.py
--rw-r--r--   0 buffer     (501) staff       (20)      367 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLLegendElement.py
--rw-r--r--   0 buffer     (501) staff       (20)      532 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLLinkElement.py
--rw-r--r--   0 buffer     (501) staff       (20)     4236 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLMediaElement.py
--rw-r--r--   0 buffer     (501) staff       (20)      264 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLMenuElement.py
--rw-r--r--   0 buffer     (501) staff       (20)      651 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLMetaElement.py
--rw-r--r--   0 buffer     (501) staff       (20)      292 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLModElement.py
--rw-r--r--   0 buffer     (501) staff       (20)      373 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLOListElement.py
--rw-r--r--   0 buffer     (501) staff       (20)     2550 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLObjectElement.py
--rw-r--r--   0 buffer     (501) staff       (20)      340 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLOptGroupElement.py
--rw-r--r--   0 buffer     (501) staff       (20)      663 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLOptionElement.py
--rw-r--r--   0 buffer     (501) staff       (20)      227 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLOptionsCollection.py
--rw-r--r--   0 buffer     (501) staff       (20)      259 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLParagraphElement.py
--rw-r--r--   0 buffer     (501) staff       (20)      364 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLParamElement.py
--rw-r--r--   0 buffer     (501) staff       (20)      258 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLPreElement.py
--rw-r--r--   0 buffer     (501) staff       (20)      253 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLQuoteElement.py
--rw-r--r--   0 buffer     (501) staff       (20)      963 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLScriptElement.py
--rw-r--r--   0 buffer     (501) staff       (20)     1594 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLSelectElement.py
--rw-r--r--   0 buffer     (501) staff       (20)      177 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLSpanElement.py
--rw-r--r--   0 buffer     (501) staff       (20)      309 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLStyleElement.py
--rw-r--r--   0 buffer     (501) staff       (20)      262 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLTableCaptionElement.py
--rw-r--r--   0 buffer     (501) staff       (20)      893 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLTableCellElement.py
--rw-r--r--   0 buffer     (501) staff       (20)      436 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLTableColElement.py
--rw-r--r--   0 buffer     (501) staff       (20)     4449 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLTableElement.py
--rw-r--r--   0 buffer     (501) staff       (20)     2865 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLTableRowElement.py
--rw-r--r--   0 buffer     (501) staff       (20)     2075 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLTableSectionElement.py
--rw-r--r--   0 buffer     (501) staff       (20)     1004 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLTextAreaElement.py
--rw-r--r--   0 buffer     (501) staff       (20)      247 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLTitleElement.py
--rw-r--r--   0 buffer     (501) staff       (20)      333 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLUListElement.py
--rw-r--r--   0 buffer     (501) staff       (20)      654 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/HTMLVideoElement.py
--rw-r--r--   0 buffer     (501) staff       (20)     1042 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/TAnimateColor.py
--rw-r--r--   0 buffer     (501) staff       (20)      281 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/TextTrackList.py
--rw-r--r--   0 buffer     (501) staff       (20)      683 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/TimeRanges.py
--rw-r--r--   0 buffer     (501) staff       (20)     4769 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/__init__.py
--rw-r--r--   0 buffer     (501) staff       (20)      462 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/attr_property.py
--rw-r--r--   0 buffer     (501) staff       (20)      418 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/bool_property.py
--rw-r--r--   0 buffer     (501) staff       (20)      463 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/form_property.py
--rw-r--r--   0 buffer     (501) staff       (20)      841 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/HTML/text_property.py
-drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.673183 thug-6.4/thug/DOM/W3C/Style/
-drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.673523 thug-6.4/thug/DOM/W3C/Style/CSS/
--rw-r--r--   0 buffer     (501) staff       (20)     1339 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Style/CSS/CSSStyleDeclaration.py
--rw-r--r--   0 buffer     (501) staff       (20)      456 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Style/CSS/ElementCSSInlineStyle.py
--rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Style/CSS/__init__.py
--rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Style/__init__.py
-drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.673862 thug-6.4/thug/DOM/W3C/URL/
--rw-r--r--   0 buffer     (501) staff       (20)     5148 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/URL/URL.py
--rw-r--r--   0 buffer     (501) staff       (20)     2728 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/URL/URLSearchParams.py
--rw-r--r--   0 buffer     (501) staff       (20)      104 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/URL/__init__.py
-drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.674233 thug-6.4/thug/DOM/W3C/Views/
--rw-r--r--   0 buffer     (501) staff       (20)      217 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Views/AbstractView.py
--rw-r--r--   0 buffer     (501) staff       (20)      211 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Views/DocumentView.py
--rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/Views/__init__.py
--rw-r--r--   0 buffer     (501) staff       (20)       34 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/__init__.py
--rw-r--r--   0 buffer     (501) staff       (20)      365 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/W3C/w3c.py
--rw-r--r--   0 buffer     (501) staff       (20)      829 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/WebStore.py
--rw-r--r--   0 buffer     (501) staff       (20)    35463 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/Window.py
--rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/__init__.py
--rw-r--r--   0 buffer     (501) staff       (20)     4750 2024-03-21 15:01:28.000000 thug-6.4/thug/DOM/w3c_bindings.py
-drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.674418 thug-6.4/thug/Encoding/
--rw-r--r--   0 buffer     (501) staff       (20)      878 2024-03-21 15:01:28.000000 thug-6.4/thug/Encoding/Encoding.py
--rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/Encoding/__init__.py
-drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.674783 thug-6.4/thug/Java/
--rw-r--r--   0 buffer     (501) staff       (20)     1109 2024-03-21 15:01:28.000000 thug-6.4/thug/Java/System.py
--rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/Java/__init__.py
--rw-r--r--   0 buffer     (501) staff       (20)      763 2024-03-21 15:01:28.000000 thug-6.4/thug/Java/java.py
--rw-r--r--   0 buffer     (501) staff       (20)      771 2024-03-21 15:01:28.000000 thug-6.4/thug/Java/lang.py
-drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.675626 thug-6.4/thug/Logging/
--rw-r--r--   0 buffer     (501) staff       (20)     2493 2024-03-21 15:01:28.000000 thug-6.4/thug/Logging/BaseLogging.py
--rw-r--r--   0 buffer     (501) staff       (20)     3897 2024-03-21 15:01:28.000000 thug-6.4/thug/Logging/Features.py
--rw-r--r--   0 buffer     (501) staff       (20)      902 2024-03-21 15:01:28.000000 thug-6.4/thug/Logging/LoggingModules.py
--rw-r--r--   0 buffer     (501) staff       (20)     4946 2024-03-21 15:01:28.000000 thug-6.4/thug/Logging/SampleLogging.py
--rw-r--r--   0 buffer     (501) staff       (20)    15290 2024-03-21 15:01:28.000000 thug-6.4/thug/Logging/ThugLogging.py
--rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/Logging/__init__.py
-drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.676559 thug-6.4/thug/Logging/modules/
--rw-r--r--   0 buffer     (501) staff       (20)     2479 2024-03-21 15:01:28.000000 thug-6.4/thug/Logging/modules/ElasticSearch.py
--rw-r--r--   0 buffer     (501) staff       (20)     1293 2024-03-21 15:01:28.000000 thug-6.4/thug/Logging/modules/ExploitGraph.py
--rw-r--r--   0 buffer     (501) staff       (20)    13218 2024-03-21 15:01:28.000000 thug-6.4/thug/Logging/modules/JSON.py
--rw-r--r--   0 buffer     (501) staff       (20)    10257 2024-03-21 15:01:28.000000 thug-6.4/thug/Logging/modules/Mapper.py
--rw-r--r--   0 buffer     (501) staff       (20)    16005 2024-03-21 15:01:28.000000 thug-6.4/thug/Logging/modules/MongoDB.py
--rw-r--r--   0 buffer     (501) staff       (20)       47 2024-03-21 15:01:28.000000 thug-6.4/thug/Logging/modules/__init__.py
-drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.676895 thug-6.4/thug/Magic/
--rw-r--r--   0 buffer     (501) staff       (20)     1592 2024-03-21 15:01:28.000000 thug-6.4/thug/Magic/Magic.py
--rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/Magic/__init__.py
-drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.677177 thug-6.4/thug/OS/
--rw-r--r--   0 buffer     (501) staff       (20)     3503 2024-03-21 15:01:28.000000 thug-6.4/thug/OS/Windows.py
--rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/OS/__init__.py
-drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.677635 thug-6.4/thug/Plugins/
--rw-r--r--   0 buffer     (501) staff       (20)      956 2024-03-21 15:01:28.000000 thug-6.4/thug/Plugins/IPlugin.py
--rw-r--r--   0 buffer     (501) staff       (20)     3438 2024-03-21 15:01:28.000000 thug-6.4/thug/Plugins/ThugPlugins.py
--rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/Plugins/__init__.py
-drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.677726 thug-6.4/thug/Plugins/plugins/
-drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.677938 thug-6.4/thug/Plugins/plugins/POST-TestPlugin-999/
--rw-r--r--   0 buffer     (501) staff       (20)      878 2024-03-21 15:01:28.000000 thug-6.4/thug/Plugins/plugins/POST-TestPlugin-999/Handler.py
--rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/Plugins/plugins/POST-TestPlugin-999/__init__.py
-drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.678144 thug-6.4/thug/Plugins/plugins/PRE-TestPlugin-999/
--rw-r--r--   0 buffer     (501) staff       (20)      878 2024-03-21 15:01:28.000000 thug-6.4/thug/Plugins/plugins/PRE-TestPlugin-999/Handler.py
--rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/Plugins/plugins/PRE-TestPlugin-999/__init__.py
--rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/Plugins/plugins/__init__.py
-drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.679514 thug-6.4/thug/ThugAPI/
--rw-r--r--   0 buffer     (501) staff       (20)    19217 2024-03-21 15:01:28.000000 thug-6.4/thug/ThugAPI/IThugAPI.py
--rw-r--r--   0 buffer     (501) staff       (20)      787 2024-03-21 15:01:28.000000 thug-6.4/thug/ThugAPI/OpaqueFilter.py
--rw-r--r--   0 buffer     (501) staff       (20)    16307 2024-03-21 15:01:28.000000 thug-6.4/thug/ThugAPI/ThugAPI.py
--rw-r--r--   0 buffer     (501) staff       (20)    10186 2024-03-21 15:01:28.000000 thug-6.4/thug/ThugAPI/ThugOpts.py
--rw-r--r--   0 buffer     (501) staff       (20)     4382 2024-03-21 15:01:28.000000 thug-6.4/thug/ThugAPI/ThugVulnModules.py
--rw-r--r--   0 buffer     (501) staff       (20)     1661 2024-03-21 15:01:28.000000 thug-6.4/thug/ThugAPI/Watchdog.py
--rw-r--r--   0 buffer     (501) staff       (20)      147 2024-03-21 15:01:28.000000 thug-6.4/thug/ThugAPI/__init__.py
--rw-r--r--   0 buffer     (501) staff       (20)      341 2024-03-21 15:01:28.000000 thug-6.4/thug/ThugAPI/abstractmethod.py
-drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.680003 thug-6.4/thug/WebTracking/
--rw-r--r--   0 buffer     (501) staff       (20)     3100 2024-03-21 15:01:28.000000 thug-6.4/thug/WebTracking/Cookies.py
--rw-r--r--   0 buffer     (501) staff       (20)     1176 2024-03-21 15:01:28.000000 thug-6.4/thug/WebTracking/WebStorage.py
--rw-r--r--   0 buffer     (501) staff       (20)     1594 2024-03-21 15:01:28.000000 thug-6.4/thug/WebTracking/WebTracking.py
--rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/WebTracking/__init__.py
--rw-r--r--   0 buffer     (501) staff       (20)     2203 2024-04-04 16:35:48.000000 thug-6.4/thug/__init__.py
-drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.680210 thug-6.4/thug/conf/
-drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.680322 thug-6.4/thug/conf/hooks/
--rw-r--r--   0 buffer     (501) staff       (20)       45 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/hooks/README
--rw-r--r--   0 buffer     (501) staff       (20)      174 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/inspector.json
-drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.685898 thug-6.4/thug/conf/personalities/
--rw-r--r--   0 buffer     (501) staff       (20)      747 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/galaxy2chrome18.json
--rw-r--r--   0 buffer     (501) staff       (20)      747 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/galaxy2chrome25.json
--rw-r--r--   0 buffer     (501) staff       (20)      743 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/galaxy2chrome29.json
--rw-r--r--   0 buffer     (501) staff       (20)      793 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/ipadchrome33.json
--rw-r--r--   0 buffer     (501) staff       (20)      739 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/ipadchrome35.json
--rw-r--r--   0 buffer     (501) staff       (20)      739 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/ipadchrome37.json
--rw-r--r--   0 buffer     (501) staff       (20)      737 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/ipadchrome38.json
--rw-r--r--   0 buffer     (501) staff       (20)      737 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/ipadchrome39.json
--rw-r--r--   0 buffer     (501) staff       (20)      737 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/ipadchrome45.json
--rw-r--r--   0 buffer     (501) staff       (20)      737 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/ipadchrome46.json
--rw-r--r--   0 buffer     (501) staff       (20)      729 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/ipadchrome47.json
--rw-r--r--   0 buffer     (501) staff       (20)      692 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/ipadsafari7.json
--rw-r--r--   0 buffer     (501) staff       (20)      688 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/ipadsafari8.json
--rw-r--r--   0 buffer     (501) staff       (20)      680 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/ipadsafari9.json
--rw-r--r--   0 buffer     (501) staff       (20)      648 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/linuxchrome26.json
--rw-r--r--   0 buffer     (501) staff       (20)      648 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/linuxchrome30.json
--rw-r--r--   0 buffer     (501) staff       (20)      648 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/linuxchrome44.json
--rw-r--r--   0 buffer     (501) staff       (20)      652 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/linuxchrome54.json
--rw-r--r--   0 buffer     (501) staff       (20)      652 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/linuxchrome98.json
--rw-r--r--   0 buffer     (501) staff       (20)      524 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/linuxfirefox19.json
--rw-r--r--   0 buffer     (501) staff       (20)      524 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/linuxfirefox40.json
--rw-r--r--   0 buffer     (501) staff       (20)      748 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/nexuschrome18.json
--rw-r--r--   0 buffer     (501) staff       (20)      679 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/osx10chrome19.json
--rw-r--r--   0 buffer     (501) staff       (20)      690 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/osx10chrome80.json
--rw-r--r--   0 buffer     (501) staff       (20)      686 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/osx10chrome97.json
--rw-r--r--   0 buffer     (501) staff       (20)      679 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/osx10safari5.json
--rw-r--r--   0 buffer     (501) staff       (20)      682 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/osx11safari14.json
--rw-r--r--   0 buffer     (501) staff       (20)      396 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/prefix_allocation.txt
--rw-r--r--   0 buffer     (501) staff       (20)     2851 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/win10edge20.json.review
--rw-r--r--   0 buffer     (501) staff       (20)     3826 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/win10ie110.json
--rw-r--r--   0 buffer     (501) staff       (20)      782 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/win2kie60.json
--rw-r--r--   0 buffer     (501) staff       (20)      915 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/win2kie80.json
--rw-r--r--   0 buffer     (501) staff       (20)      686 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/win7chrome20.json
--rw-r--r--   0 buffer     (501) staff       (20)      686 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/win7chrome40.json
--rw-r--r--   0 buffer     (501) staff       (20)      686 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/win7chrome45.json
--rw-r--r--   0 buffer     (501) staff       (20)      686 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/win7chrome49.json
--rw-r--r--   0 buffer     (501) staff       (20)      579 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/win7firefox3.json
--rw-r--r--   0 buffer     (501) staff       (20)     3769 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/win7ie100.json
--rw-r--r--   0 buffer     (501) staff       (20)     3800 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/win7ie80.json
--rw-r--r--   0 buffer     (501) staff       (20)     3820 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/win7ie90.json
--rw-r--r--   0 buffer     (501) staff       (20)      678 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/win7safari5.json
--rw-r--r--   0 buffer     (501) staff       (20)      674 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/winxpchrome20.json
--rw-r--r--   0 buffer     (501) staff       (20)      564 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/winxpfirefox12.json
--rw-r--r--   0 buffer     (501) staff       (20)     2876 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/winxpie60.json
--rw-r--r--   0 buffer     (501) staff       (20)     2896 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/winxpie61.json
--rw-r--r--   0 buffer     (501) staff       (20)     2871 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/winxpie70.json
--rw-r--r--   0 buffer     (501) staff       (20)     2968 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/winxpie80.json
--rw-r--r--   0 buffer     (501) staff       (20)      666 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/personalities/winxpsafari5.json
-drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.686010 thug-6.4/thug/conf/plugins/
--rw-r--r--   0 buffer     (501) staff       (20)       47 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/plugins/README
-drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.687280 thug-6.4/thug/conf/rules/
-drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.687356 thug-6.4/thug/conf/rules/cookieclassifier/
--rw-r--r--   0 buffer     (501) staff       (20)      117 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/cookieclassifier/README
--rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/cookieclassifier.yar
-drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.687469 thug-6.4/thug/conf/rules/cookiefilter/
--rw-r--r--   0 buffer     (501) staff       (20)      105 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/cookiefilter/README
--rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/cookiefilter.yar
-drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.687578 thug-6.4/thug/conf/rules/htmlclassifier/
--rw-r--r--   0 buffer     (501) staff       (20)      113 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/htmlclassifier/README
--rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/htmlclassifier.yar
-drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.687689 thug-6.4/thug/conf/rules/htmlfilter/
--rw-r--r--   0 buffer     (501) staff       (20)      101 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/htmlfilter/README
--rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/htmlfilter.yar
-drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.687804 thug-6.4/thug/conf/rules/imageclassifier/
--rw-r--r--   0 buffer     (501) staff       (20)      115 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/imageclassifier/README
--rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/imageclassifier.yar
-drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.687924 thug-6.4/thug/conf/rules/imagefilter/
--rw-r--r--   0 buffer     (501) staff       (20)      103 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/imagefilter/README
--rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/imagefilter.yar
-drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.688035 thug-6.4/thug/conf/rules/jsclassifier/
--rw-r--r--   0 buffer     (501) staff       (20)      245 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/jsclassifier/plugindetect.yar
--rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/jsclassifier.yar
-drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.688147 thug-6.4/thug/conf/rules/jsfilter/
--rw-r--r--   0 buffer     (501) staff       (20)       97 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/jsfilter/README
--rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/jsfilter.yar
-drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.688261 thug-6.4/thug/conf/rules/sampleclassifier/
--rw-r--r--   0 buffer     (501) staff       (20)      117 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/sampleclassifier/README
--rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/sampleclassifier.yar
-drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.688388 thug-6.4/thug/conf/rules/samplefilter/
--rw-r--r--   0 buffer     (501) staff       (20)      105 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/samplefilter/README
--rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/samplefilter.yar
-drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.688503 thug-6.4/thug/conf/rules/textclassifier/
--rw-r--r--   0 buffer     (501) staff       (20)      113 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/textclassifier/README
--rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/textclassifier.yar
-drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.688615 thug-6.4/thug/conf/rules/textfilter/
--rw-r--r--   0 buffer     (501) staff       (20)      101 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/textfilter/README
--rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/textfilter.yar
-drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.690628 thug-6.4/thug/conf/rules/urlclassifier/
--rw-r--r--   0 buffer     (501) staff       (20)      111 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/urlclassifier/README
--rw-r--r--   0 buffer     (501) staff       (20)     3005 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/urlclassifier/blackhole.yar
--rw-r--r--   0 buffer     (501) staff       (20)      418 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/urlclassifier/cool.yar
--rw-r--r--   0 buffer     (501) staff       (20)      766 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/urlclassifier/crimeboss.yar
--rw-r--r--   0 buffer     (501) staff       (20)      641 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/urlclassifier/critxpack.yar
--rw-r--r--   0 buffer     (501) staff       (20)     1000 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/urlclassifier/fiesta.yar
--rw-r--r--   0 buffer     (501) staff       (20)      870 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/urlclassifier/g01pack.yar
--rw-r--r--   0 buffer     (501) staff       (20)      387 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/urlclassifier/impact.yar
--rw-r--r--   0 buffer     (501) staff       (20)      808 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/urlclassifier/neutrino.yar
--rw-r--r--   0 buffer     (501) staff       (20)      612 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/urlclassifier/nuclear.yar
--rw-r--r--   0 buffer     (501) staff       (20)      969 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/urlclassifier/popads.yar
--rw-r--r--   0 buffer     (501) staff       (20)      765 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/urlclassifier/redkit.yar
--rw-r--r--   0 buffer     (501) staff       (20)      427 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/urlclassifier/safepack.yar
--rw-r--r--   0 buffer     (501) staff       (20)      176 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/urlclassifier/sakura.yar
--rw-r--r--   0 buffer     (501) staff       (20)      478 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/urlclassifier/sofosfo.yar
--rw-r--r--   0 buffer     (501) staff       (20)     2400 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/urlclassifier/styx.yar
--rw-r--r--   0 buffer     (501) staff       (20)      849 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/urlclassifier/sweetorange.yar
--rw-r--r--   0 buffer     (501) staff       (20)      340 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/urlclassifier/tds.yar
--rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/urlclassifier.yar
-drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.690757 thug-6.4/thug/conf/rules/urlfilter/
--rw-r--r--   0 buffer     (501) staff       (20)       99 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/urlfilter/README
--rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/urlfilter.yar
-drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.690873 thug-6.4/thug/conf/rules/vbsclassifier/
--rw-r--r--   0 buffer     (501) staff       (20)      111 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/vbsclassifier/README
--rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/vbsclassifier.yar
-drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.690983 thug-6.4/thug/conf/rules/vbsfilter/
--rw-r--r--   0 buffer     (501) staff       (20)       99 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/vbsfilter/README
--rw-r--r--   0 buffer     (501) staff       (20)        0 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/rules/vbsfilter.yar
-drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.691900 thug-6.4/thug/conf/scripts/
--rw-r--r--   0 buffer     (501) staff       (20)     3837 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/scripts/atob.js
--rw-r--r--   0 buffer     (501) staff       (20)     1821 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/scripts/btoa.js
--rw-r--r--   0 buffer     (501) staff       (20)       69 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/scripts/date.js
--rw-r--r--   0 buffer     (501) staff       (20)      197 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/scripts/eval.js
--rw-r--r--   0 buffer     (501) staff       (20)       87 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/scripts/message-event.js
--rw-r--r--   0 buffer     (501) staff       (20)      204 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/scripts/storage.js
--rw-r--r--   0 buffer     (501) staff       (20)      753 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/scripts/thug.js
--rw-r--r--   0 buffer     (501) staff       (20)      205 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/scripts/write.js
--rw-r--r--   0 buffer     (501) staff       (20)      325 2024-03-21 15:01:28.000000 thug-6.4/thug/conf/thug.conf
--rw-r--r--   0 buffer     (501) staff       (20)    19877 2024-03-21 15:01:28.000000 thug-6.4/thug/thug.py
-drwxr-xr-x   0 buffer     (501) staff       (20)        0 2024-04-04 17:17:07.692071 thug-6.4/thug.egg-info/
--rw-r--r--   0 buffer     (501) staff       (20)     5535 2024-04-04 17:17:07.000000 thug-6.4/thug.egg-info/PKG-INFO
--rw-r--r--   0 buffer     (501) staff       (20)    15909 2024-04-04 17:17:07.000000 thug-6.4/thug.egg-info/SOURCES.txt
--rw-r--r--   0 buffer     (501) staff       (20)        1 2024-04-04 17:17:07.000000 thug-6.4/thug.egg-info/dependency_links.txt
--rw-r--r--   0 buffer     (501) staff       (20)       40 2024-04-04 17:17:07.000000 thug-6.4/thug.egg-info/entry_points.txt
--rw-r--r--   0 buffer     (501) staff       (20)      694 2024-04-04 17:17:07.000000 thug-6.4/thug.egg-info/requires.txt
--rw-r--r--   0 buffer     (501) staff       (20)       10 2024-04-04 17:17:07.000000 thug-6.4/thug.egg-info/top_level.txt
--rw-r--r--   0 buffer     (501) staff       (20)        1 2024-04-04 17:17:07.000000 thug-6.4/thug.egg-info/zip-safe
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.856458 thug-6.5/
+-rw-r--r--   0 buffer    (1000) buffer    (1000)    17987 2022-11-28 09:02:06.000000 thug-6.5/LICENSE.txt
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      130 2023-01-12 15:47:27.000000 thug-6.5/MANIFEST.in
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     5613 2024-04-11 14:03:15.855458 thug-6.5/PKG-INFO
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     2695 2024-01-19 09:00:07.000000 thug-6.5/README.rst
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     3816 2024-04-11 13:56:54.000000 thug-6.5/pyproject.toml
+-rw-r--r--   0 buffer    (1000) buffer    (1000)       38 2024-04-11 14:03:15.856458 thug-6.5/setup.cfg
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.735456 thug-6.5/thug/
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.737456 thug-6.5/thug/ActiveX/
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     7458 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/ActiveX.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)    47758 2024-04-11 13:56:54.000000 thug-6.5/thug/ActiveX/CLSID.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.5/thug/ActiveX/__init__.py
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.764456 thug-6.5/thug/ActiveX/modules/
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      323 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/AOLAttack.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      871 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/AcroPDF.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      610 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/AdodbRecordset.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     2404 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/AdodbStream.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     1275 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/AnswerWorks.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      948 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/AolAmpX.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      736 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/AolICQ.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      620 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/BaiduBar.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      498 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/BitDefender.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      360 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/CABrightStor.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      531 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/CGAgent.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      446 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/Comodo.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      652 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/ConnectAndEnterRoom.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      245 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/CreativeSoftAttack.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      408 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/DLinkMPEG.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      605 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/DPClient.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      411 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/DVRHOSTWeb.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      548 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/DirectShow.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      342 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/DivX.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     1651 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/Domino.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     1170 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/EnjoySAP.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      751 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/FacebookPhotoUploader.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     3094 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/File.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      441 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/FileUploader.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     2252 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/Folder.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      460 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/GLIEDown2.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      677 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/GatewayWeblaunch.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      383 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/Gogago.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      492 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/GomWeb.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     2728 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/HPInfo.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      407 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/ICQToolbar.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      807 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/IMWebControl.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      413 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/InternetCleverSuite.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     1750 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/JavaDeploymentToolkit.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      932 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/JetAudioDownloadFromMusicStore.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      368 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/Kingsoft.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      652 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/MSRICHTXT.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      411 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/MSVFP.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      457 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/MSXML2DOMDocument.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     3549 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/MacrovisionFlexNet.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      295 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/MicrosoftWorks7Attack.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     2119 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/MicrosoftXMLDOM.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     7787 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/MicrosoftXMLHTTP.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      430 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/Move.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      376 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/MyspaceUploader.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      520 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/NCTAudioFile2.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      972 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/NamoInstaller.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      547 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/NeoTracePro.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     2210 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/NessusScanCtrl.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      945 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/OfficeOCX.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      919 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/OurgameGLWorld.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     1066 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/PPlayer.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      462 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/PTZCamPanel.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      458 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/QuantumStreaming.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      447 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/QvodCtrl.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      712 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/RDSDataSpace.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     2063 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/RealPlayer.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      285 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/RediffBolDownloaderAttack.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      684 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/RegistryPro.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      316 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/RisingScanner.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      412 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/RtspVaPgCtrl.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      980 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/SSReaderPdg2.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     1032 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/ScriptingDictionary.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      342 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/ScriptingEncoder.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     4975 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/ScriptingFileSystemObject.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     1184 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/ShellApplication.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      298 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/Shockwave.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      390 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/ShockwaveFlash10.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      390 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/ShockwaveFlash11.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      390 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/ShockwaveFlash12.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      390 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/ShockwaveFlash9.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      274 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/SilverLight.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      752 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/SinaDLoader.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     1165 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/SnapshotViewer.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      646 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/SonicWallNetExtenderAddRouteEntry.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      754 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/Spreadsheet.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      609 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/StormConfig.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     2028 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/StormMps.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      480 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/StreamAudioChainCast.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      854 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/SymantecAppStream.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     1949 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/SymantecBackupExec.py
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.764456 thug-6.5/thug/ActiveX/modules/System/
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.764456 thug-6.5/thug/ActiveX/modules/System/Collections/
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      353 2024-04-11 13:56:54.000000 thug-6.5/thug/ActiveX/modules/System/Collections/ArrayList.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)       56 2024-04-11 13:56:54.000000 thug-6.5/thug/ActiveX/modules/System/Collections/__init__.py
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.765456 thug-6.5/thug/ActiveX/modules/System/IO/
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      443 2024-04-11 13:56:54.000000 thug-6.5/thug/ActiveX/modules/System/IO/MemoryStream.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)       62 2024-04-11 13:56:54.000000 thug-6.5/thug/ActiveX/modules/System/IO/__init__.py
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.766456 thug-6.5/thug/ActiveX/modules/System/Runtime/
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      134 2024-04-11 13:56:54.000000 thug-6.5/thug/ActiveX/modules/System/Runtime/Activator.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      173 2024-04-11 13:56:54.000000 thug-6.5/thug/ActiveX/modules/System/Runtime/Delegate.py
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.766456 thug-6.5/thug/ActiveX/modules/System/Runtime/Serialization/
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.766456 thug-6.5/thug/ActiveX/modules/System/Runtime/Serialization/Formatters/
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.767456 thug-6.5/thug/ActiveX/modules/System/Runtime/Serialization/Formatters/Binary/
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      341 2024-04-11 13:56:54.000000 thug-6.5/thug/ActiveX/modules/System/Runtime/Serialization/Formatters/Binary/BinaryFormatter.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)       68 2024-04-11 13:56:54.000000 thug-6.5/thug/ActiveX/modules/System/Runtime/Serialization/Formatters/Binary/__init__.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)       50 2024-04-11 13:56:54.000000 thug-6.5/thug/ActiveX/modules/System/Runtime/Serialization/Formatters/__init__.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)       58 2024-04-11 13:56:54.000000 thug-6.5/thug/ActiveX/modules/System/Runtime/Serialization/__init__.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)       64 2024-04-11 13:56:54.000000 thug-6.5/thug/ActiveX/modules/System/Runtime/__init__.py
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.767456 thug-6.5/thug/ActiveX/modules/System/Security/
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.767456 thug-6.5/thug/ActiveX/modules/System/Security/Cryptography/
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      323 2024-04-11 13:56:54.000000 thug-6.5/thug/ActiveX/modules/System/Security/Cryptography/FromBase64Transform.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)       76 2024-04-11 13:56:54.000000 thug-6.5/thug/ActiveX/modules/System/Security/Cryptography/__init__.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)       62 2024-04-11 13:56:54.000000 thug-6.5/thug/ActiveX/modules/System/Security/__init__.py
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.768456 thug-6.5/thug/ActiveX/modules/System/Text/
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      388 2024-04-11 13:56:54.000000 thug-6.5/thug/ActiveX/modules/System/Text/ASCIIEncoding.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)       64 2024-04-11 13:56:54.000000 thug-6.5/thug/ActiveX/modules/System/Text/__init__.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      171 2024-04-11 13:56:54.000000 thug-6.5/thug/ActiveX/modules/System/__init__.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     4792 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/TextStream.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      713 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/Toshiba.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      330 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/UUSeeUpdate.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      502 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/UniversalUpload.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     1445 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/VLC.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      527 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/VisualStudioDTE80.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      493 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/VsaIDEDTE.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      493 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/VsmIDEDTE.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      815 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/WMEncProfileManager.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      132 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/WMP.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      257 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/WScriptCollection.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     1279 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/WScriptExec.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     1726 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/WScriptNetwork.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     8198 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/WScriptShell.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      218 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/WScriptShortcut.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      590 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/WebViewFolderIcon.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     1358 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/WinNTSystemInfo.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      530 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/WinZip.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      145 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/WindowsMediaPlayer.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      921 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/XMLDOMParseError.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      888 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/XUpload.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      976 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/YahooJukebox.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      446 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/YahooMessengerCyft.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      939 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/YahooMessengerYVerInfo.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     1102 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/YahooMessengerYwcvwr.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     1660 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/ZenturiProgramCheckerAttack.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     2079 2024-01-17 12:09:54.000000 thug-6.5/thug/ActiveX/modules/__init__.py
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.768456 thug-6.5/thug/Analysis/
+-rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.5/thug/Analysis/__init__.py
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.768456 thug-6.5/thug/Analysis/awis/
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     3488 2024-01-17 12:09:54.000000 thug-6.5/thug/Analysis/awis/AWIS.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.5/thug/Analysis/awis/__init__.py
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.769456 thug-6.5/thug/Analysis/context/
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     1609 2024-01-17 12:09:54.000000 thug-6.5/thug/Analysis/context/ContextAnalyzer.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.5/thug/Analysis/context/__init__.py
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.769456 thug-6.5/thug/Analysis/favicon/
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      394 2024-01-17 12:09:54.000000 thug-6.5/thug/Analysis/favicon/Favicon.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-09-11 08:32:02.000000 thug-6.5/thug/Analysis/favicon/__init__.py
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.770456 thug-6.5/thug/Analysis/honeyagent/
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     3980 2024-01-17 12:09:54.000000 thug-6.5/thug/Analysis/honeyagent/HoneyAgent.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.5/thug/Analysis/honeyagent/__init__.py
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.770456 thug-6.5/thug/Analysis/screenshot/
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     1309 2024-01-17 12:09:54.000000 thug-6.5/thug/Analysis/screenshot/Screenshot.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.5/thug/Analysis/screenshot/__init__.py
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.771456 thug-6.5/thug/Analysis/shellcode/
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     8118 2024-01-17 12:09:54.000000 thug-6.5/thug/Analysis/shellcode/Shellcode.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.5/thug/Analysis/shellcode/__init__.py
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.772456 thug-6.5/thug/Classifier/
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     5394 2024-01-17 12:09:54.000000 thug-6.5/thug/Classifier/BaseClassifier.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     2094 2024-01-17 12:09:54.000000 thug-6.5/thug/Classifier/CookieClassifier.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     2147 2024-01-17 12:09:54.000000 thug-6.5/thug/Classifier/HTMLClassifier.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     2057 2024-01-17 12:09:54.000000 thug-6.5/thug/Classifier/ImageClassifier.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     1996 2024-01-17 12:09:54.000000 thug-6.5/thug/Classifier/JSClassifier.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     2230 2024-01-17 12:09:54.000000 thug-6.5/thug/Classifier/SampleClassifier.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     2070 2024-01-17 12:09:54.000000 thug-6.5/thug/Classifier/TextClassifier.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     2318 2024-01-17 12:09:54.000000 thug-6.5/thug/Classifier/URLClassifier.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     2002 2024-01-17 12:09:54.000000 thug-6.5/thug/Classifier/VBSClassifier.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.5/thug/Classifier/__init__.py
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.781457 thug-6.5/thug/DOM/
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     2327 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/Alexa.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     2236 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/AsyncPrefetcher.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     2298 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/CCInterpreter.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      878 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/Chrome.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     1302 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/ClipboardData.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      817 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/Components.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     5685 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/Console.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     1113 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/Crypto.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)    56116 2024-02-09 06:17:13.000000 thug-6.5/thug/DOM/DFT.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     3511 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/External.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     2831 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/HTMLInspector.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)    10997 2024-02-22 09:16:59.000000 thug-6.5/thug/DOM/HTTPSession.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      932 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/HTTPSessionException.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     3717 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/History.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     3501 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/JSClass.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     8294 2024-02-09 06:17:13.000000 thug-6.5/thug/DOM/JSEngine.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     4395 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/JSInspector.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     5971 2024-04-11 13:56:54.000000 thug-6.5/thug/DOM/JScriptEncode.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      752 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/LocalStorage.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     4873 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/Location.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)    18649 2024-02-09 06:17:13.000000 thug-6.5/thug/DOM/MIMEHandler.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      762 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/Map.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     1195 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/MimeType.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     4504 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/MimeTypes.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      782 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/MozConnection.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)    13892 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/Navigator.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     4191 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/Personality.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     1231 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/Plugin.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     1469 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/Plugins.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     1064 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/SchemeHandler.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     5954 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/Screen.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      756 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/SessionStorage.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     1775 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/Sidebar.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     2830 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/Storage.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     2805 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/UserProfile.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      766 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/Utils.py
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.782456 thug-6.5/thug/DOM/W3C/
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.788457 thug-6.5/thug/DOM/W3C/Core/
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     2172 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Core/Attr.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      266 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Core/CDATASection.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     1245 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Core/CharacterData.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     3760 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Core/ClassList.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      565 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Core/Comment.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     1893 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Core/DOMException.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     4988 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Core/DOMImplementation.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     8842 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Core/Document.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     2422 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Core/DocumentFragment.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     1512 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Core/DocumentType.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     9703 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Core/Element.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      458 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Core/Entity.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      501 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Core/EntityReference.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     1295 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Core/NamedNodeMap.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)    14383 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Core/Node.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      617 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Core/NodeList.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      341 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Core/NodeType.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      486 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Core/Notation.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      507 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Core/ProcessingInstruction.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      804 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Core/Text.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      939 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Core/__init__.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      362 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Core/abstractmethod.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      274 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/DOMParser.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     1453 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/DOMTokenList.py
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.790457 thug-6.5/thug/DOM/W3C/Events/
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      828 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Events/DocumentEvent.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     4094 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Events/Event.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      477 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Events/EventException.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      274 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Events/EventListener.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     9365 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Events/EventTarget.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      389 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Events/HTMLEvent.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     1174 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Events/MessageEvent.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     2068 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Events/MouseEvent.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     1557 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Events/MutationEvent.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     1113 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Events/StorageEvent.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      634 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Events/UIEvent.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      628 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Events/__init__.py
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.791457 thug-6.5/thug/DOM/W3C/File/
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     2380 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/File/Blob.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     1377 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/File/File.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)       74 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/File/__init__.py
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.813457 thug-6.5/thug/DOM/W3C/HTML/
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      194 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/W3C/HTML/AudioTrackList.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      611 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/Dataset.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      374 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLAllCollection.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     1878 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLAnchorElement.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      626 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLAppletElement.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      247 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLAudioElement.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      252 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLBRElement.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      289 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLBaseElement.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      329 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLBaseFontElement.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     1484 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLBodyElement.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      561 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLButtonElement.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     1278 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLCollection.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      265 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLDListElement.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      263 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLDirectoryElement.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      253 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLDivElement.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)    16355 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLDocument.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      952 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLDocumentCompatibleInfo.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      412 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLDocumentCompatibleInfoCollection.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     4438 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLElement.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      332 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLFieldSetElement.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      320 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLFontElement.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      204 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLFormControlsCollection.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     1689 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLFormElement.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      948 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLFrameElement.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      289 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLFrameSetElement.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      400 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLHRElement.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      258 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLHeadElement.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      257 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLHeadingElement.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      258 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLHtmlElement.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     1219 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLIFrameElement.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     1233 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLImageElement.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     1330 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLInputElement.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      275 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLIsIndexElement.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      290 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLLIElement.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      366 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLLabelElement.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      367 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLLegendElement.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      532 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLLinkElement.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     4236 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLMediaElement.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      264 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLMenuElement.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      651 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLMetaElement.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      292 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLModElement.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      373 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLOListElement.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     2550 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLObjectElement.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      340 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLOptGroupElement.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      663 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLOptionElement.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      227 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLOptionsCollection.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      259 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLParagraphElement.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      364 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLParamElement.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      258 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLPreElement.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      253 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLQuoteElement.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      963 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLScriptElement.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     1594 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLSelectElement.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      177 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLSpanElement.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      309 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLStyleElement.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      262 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLTableCaptionElement.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      893 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLTableCellElement.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      436 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLTableColElement.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     4449 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLTableElement.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     2865 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLTableRowElement.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     2075 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLTableSectionElement.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     1004 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLTextAreaElement.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      247 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLTitleElement.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      333 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLUListElement.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      654 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/HTMLVideoElement.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     1042 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/TAnimateColor.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      281 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/TextTrackList.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      683 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/TimeRanges.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     4769 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/__init__.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      462 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/attr_property.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      418 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/bool_property.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      463 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/form_property.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      841 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/HTML/text_property.py
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.813457 thug-6.5/thug/DOM/W3C/Style/
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.814457 thug-6.5/thug/DOM/W3C/Style/CSS/
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     1339 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Style/CSS/CSSStyleDeclaration.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      456 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Style/CSS/ElementCSSInlineStyle.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/W3C/Style/CSS/__init__.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/W3C/Style/__init__.py
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.814457 thug-6.5/thug/DOM/W3C/URL/
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     5148 2024-02-09 06:17:13.000000 thug-6.5/thug/DOM/W3C/URL/URL.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     2728 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/URL/URLSearchParams.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      104 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/URL/__init__.py
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.815457 thug-6.5/thug/DOM/W3C/Views/
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      217 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/W3C/Views/AbstractView.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      211 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/Views/DocumentView.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/W3C/Views/__init__.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)       34 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/__init__.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      365 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/W3C/w3c.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      829 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/WebStore.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)    35463 2024-02-09 06:17:13.000000 thug-6.5/thug/DOM/Window.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.5/thug/DOM/__init__.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     4750 2024-01-17 12:09:54.000000 thug-6.5/thug/DOM/w3c_bindings.py
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.816457 thug-6.5/thug/Encoding/
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      878 2024-01-17 12:09:54.000000 thug-6.5/thug/Encoding/Encoding.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.5/thug/Encoding/__init__.py
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.816457 thug-6.5/thug/Java/
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     1109 2024-01-17 12:09:54.000000 thug-6.5/thug/Java/System.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.5/thug/Java/__init__.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      763 2022-11-28 09:02:06.000000 thug-6.5/thug/Java/java.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      771 2022-11-28 09:02:06.000000 thug-6.5/thug/Java/lang.py
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.818457 thug-6.5/thug/Logging/
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     2493 2024-01-17 12:09:54.000000 thug-6.5/thug/Logging/BaseLogging.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     3897 2024-01-17 12:09:54.000000 thug-6.5/thug/Logging/Features.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      902 2024-01-17 12:09:54.000000 thug-6.5/thug/Logging/LoggingModules.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     4946 2024-01-17 12:09:54.000000 thug-6.5/thug/Logging/SampleLogging.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)    15290 2024-02-09 06:17:13.000000 thug-6.5/thug/Logging/ThugLogging.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.5/thug/Logging/__init__.py
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.820457 thug-6.5/thug/Logging/modules/
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     2479 2024-01-17 12:09:54.000000 thug-6.5/thug/Logging/modules/ElasticSearch.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     1293 2024-01-17 12:09:54.000000 thug-6.5/thug/Logging/modules/ExploitGraph.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)    13218 2024-01-17 12:09:54.000000 thug-6.5/thug/Logging/modules/JSON.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)    10257 2024-01-17 12:09:54.000000 thug-6.5/thug/Logging/modules/Mapper.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)    16005 2024-01-17 12:09:54.000000 thug-6.5/thug/Logging/modules/MongoDB.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)       47 2024-01-17 12:09:54.000000 thug-6.5/thug/Logging/modules/__init__.py
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.820457 thug-6.5/thug/Magic/
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     1592 2024-01-17 12:09:54.000000 thug-6.5/thug/Magic/Magic.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.5/thug/Magic/__init__.py
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.820457 thug-6.5/thug/OS/
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     3503 2024-01-17 12:09:54.000000 thug-6.5/thug/OS/Windows.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.5/thug/OS/__init__.py
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.821457 thug-6.5/thug/Plugins/
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      956 2022-11-28 09:02:06.000000 thug-6.5/thug/Plugins/IPlugin.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     3438 2024-01-17 12:09:54.000000 thug-6.5/thug/Plugins/ThugPlugins.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.5/thug/Plugins/__init__.py
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.821457 thug-6.5/thug/Plugins/plugins/
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.822457 thug-6.5/thug/Plugins/plugins/POST-TestPlugin-999/
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      878 2022-11-28 09:02:06.000000 thug-6.5/thug/Plugins/plugins/POST-TestPlugin-999/Handler.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.5/thug/Plugins/plugins/POST-TestPlugin-999/__init__.py
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.822457 thug-6.5/thug/Plugins/plugins/PRE-TestPlugin-999/
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      878 2022-11-28 09:02:06.000000 thug-6.5/thug/Plugins/plugins/PRE-TestPlugin-999/Handler.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.5/thug/Plugins/plugins/PRE-TestPlugin-999/__init__.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.5/thug/Plugins/plugins/__init__.py
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.824457 thug-6.5/thug/ThugAPI/
+-rw-r--r--   0 buffer    (1000) buffer    (1000)    19217 2024-02-22 09:16:59.000000 thug-6.5/thug/ThugAPI/IThugAPI.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      787 2022-11-28 09:02:06.000000 thug-6.5/thug/ThugAPI/OpaqueFilter.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)    16307 2024-02-22 09:16:59.000000 thug-6.5/thug/ThugAPI/ThugAPI.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)    10186 2024-02-22 09:16:59.000000 thug-6.5/thug/ThugAPI/ThugOpts.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     4382 2024-01-17 12:09:54.000000 thug-6.5/thug/ThugAPI/ThugVulnModules.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     1661 2024-01-17 12:09:54.000000 thug-6.5/thug/ThugAPI/Watchdog.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      147 2024-01-17 12:09:54.000000 thug-6.5/thug/ThugAPI/__init__.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      341 2024-01-17 12:09:54.000000 thug-6.5/thug/ThugAPI/abstractmethod.py
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.825457 thug-6.5/thug/WebTracking/
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     3100 2024-01-17 12:09:54.000000 thug-6.5/thug/WebTracking/Cookies.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     1176 2022-11-28 09:02:06.000000 thug-6.5/thug/WebTracking/WebStorage.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     1594 2024-01-17 12:09:54.000000 thug-6.5/thug/WebTracking/WebTracking.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2022-11-28 09:02:06.000000 thug-6.5/thug/WebTracking/__init__.py
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     2203 2024-04-11 13:56:54.000000 thug-6.5/thug/__init__.py
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.826457 thug-6.5/thug/conf/
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.826457 thug-6.5/thug/conf/hooks/
+-rw-r--r--   0 buffer    (1000) buffer    (1000)       45 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/hooks/README
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      174 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/inspector.json
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.837458 thug-6.5/thug/conf/personalities/
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      747 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/galaxy2chrome18.json
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      747 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/galaxy2chrome25.json
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      743 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/galaxy2chrome29.json
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      793 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/ipadchrome33.json
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      739 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/ipadchrome35.json
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      739 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/ipadchrome37.json
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      737 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/ipadchrome38.json
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      737 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/ipadchrome39.json
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      737 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/ipadchrome45.json
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      737 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/ipadchrome46.json
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      729 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/ipadchrome47.json
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      692 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/ipadsafari7.json
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      688 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/ipadsafari8.json
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      680 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/ipadsafari9.json
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      648 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/linuxchrome26.json
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      648 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/linuxchrome30.json
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      648 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/linuxchrome44.json
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      652 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/linuxchrome54.json
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      652 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/linuxchrome98.json
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      524 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/linuxfirefox19.json
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      524 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/linuxfirefox40.json
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      748 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/nexuschrome18.json
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      679 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/osx10chrome19.json
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      690 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/osx10chrome80.json
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      686 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/osx10chrome97.json
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      679 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/osx10safari5.json
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      682 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/osx11safari14.json
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      396 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/prefix_allocation.txt
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     2851 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/win10edge20.json.review
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     3826 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/win10ie110.json
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      782 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/win2kie60.json
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      915 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/win2kie80.json
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      686 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/win7chrome20.json
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      686 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/win7chrome40.json
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      686 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/win7chrome45.json
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      686 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/win7chrome49.json
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      579 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/win7firefox3.json
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     3769 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/win7ie100.json
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     3800 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/win7ie80.json
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     3820 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/win7ie90.json
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      678 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/win7safari5.json
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      674 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/winxpchrome20.json
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      564 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/winxpfirefox12.json
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     2876 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/winxpie60.json
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     2896 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/winxpie61.json
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     2871 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/winxpie70.json
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     2968 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/winxpie80.json
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      666 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/personalities/winxpsafari5.json
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.837458 thug-6.5/thug/conf/plugins/
+-rw-r--r--   0 buffer    (1000) buffer    (1000)       47 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/plugins/README
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.841457 thug-6.5/thug/conf/rules/
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.841457 thug-6.5/thug/conf/rules/cookieclassifier/
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      117 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/cookieclassifier/README
+-rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/cookieclassifier.yar
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.841457 thug-6.5/thug/conf/rules/cookiefilter/
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      105 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/cookiefilter/README
+-rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/cookiefilter.yar
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.841457 thug-6.5/thug/conf/rules/htmlclassifier/
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      113 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/htmlclassifier/README
+-rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/htmlclassifier.yar
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.842457 thug-6.5/thug/conf/rules/htmlfilter/
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      101 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/htmlfilter/README
+-rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/htmlfilter.yar
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.842457 thug-6.5/thug/conf/rules/imageclassifier/
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      115 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/imageclassifier/README
+-rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/imageclassifier.yar
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.842457 thug-6.5/thug/conf/rules/imagefilter/
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      103 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/imagefilter/README
+-rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/imagefilter.yar
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.842457 thug-6.5/thug/conf/rules/jsclassifier/
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      245 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/jsclassifier/plugindetect.yar
+-rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/jsclassifier.yar
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.843458 thug-6.5/thug/conf/rules/jsfilter/
+-rw-r--r--   0 buffer    (1000) buffer    (1000)       97 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/jsfilter/README
+-rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/jsfilter.yar
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.843458 thug-6.5/thug/conf/rules/sampleclassifier/
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      117 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/sampleclassifier/README
+-rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/sampleclassifier.yar
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.843458 thug-6.5/thug/conf/rules/samplefilter/
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      105 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/samplefilter/README
+-rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/samplefilter.yar
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.843458 thug-6.5/thug/conf/rules/textclassifier/
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      113 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/textclassifier/README
+-rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/textclassifier.yar
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.844457 thug-6.5/thug/conf/rules/textfilter/
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      101 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/textfilter/README
+-rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/textfilter.yar
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.848458 thug-6.5/thug/conf/rules/urlclassifier/
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      111 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/urlclassifier/README
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     3005 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/urlclassifier/blackhole.yar
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      418 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/urlclassifier/cool.yar
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      766 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/urlclassifier/crimeboss.yar
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      641 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/urlclassifier/critxpack.yar
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     1000 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/urlclassifier/fiesta.yar
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      870 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/urlclassifier/g01pack.yar
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      387 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/urlclassifier/impact.yar
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      808 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/urlclassifier/neutrino.yar
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      612 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/urlclassifier/nuclear.yar
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      969 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/urlclassifier/popads.yar
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      765 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/urlclassifier/redkit.yar
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      427 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/urlclassifier/safepack.yar
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      176 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/urlclassifier/sakura.yar
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      478 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/urlclassifier/sofosfo.yar
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     2400 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/urlclassifier/styx.yar
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      849 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/urlclassifier/sweetorange.yar
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      340 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/urlclassifier/tds.yar
+-rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/urlclassifier.yar
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.848458 thug-6.5/thug/conf/rules/urlfilter/
+-rw-r--r--   0 buffer    (1000) buffer    (1000)       99 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/urlfilter/README
+-rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/urlfilter.yar
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.848458 thug-6.5/thug/conf/rules/vbsclassifier/
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      111 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/vbsclassifier/README
+-rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/vbsclassifier.yar
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.849458 thug-6.5/thug/conf/rules/vbsfilter/
+-rw-r--r--   0 buffer    (1000) buffer    (1000)       99 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/vbsfilter/README
+-rw-r--r--   0 buffer    (1000) buffer    (1000)        0 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/rules/vbsfilter.yar
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.850458 thug-6.5/thug/conf/scripts/
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     3837 2024-02-09 06:17:13.000000 thug-6.5/thug/conf/scripts/atob.js
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     1821 2024-02-09 06:17:13.000000 thug-6.5/thug/conf/scripts/btoa.js
+-rw-r--r--   0 buffer    (1000) buffer    (1000)       69 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/scripts/date.js
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      197 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/scripts/eval.js
+-rw-r--r--   0 buffer    (1000) buffer    (1000)       87 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/scripts/message-event.js
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      204 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/scripts/storage.js
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      753 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/scripts/thug.js
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      205 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/scripts/write.js
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      325 2023-01-12 15:47:27.000000 thug-6.5/thug/conf/thug.conf
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.852458 thug-6.5/thug/thug.egg-info/
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     4017 2022-12-08 08:47:59.000000 thug-6.5/thug/thug.egg-info/PKG-INFO
+-rw-r--r--   0 buffer    (1000) buffer    (1000)    19264 2022-12-08 08:47:59.000000 thug-6.5/thug/thug.egg-info/SOURCES.txt
+-rw-r--r--   0 buffer    (1000) buffer    (1000)        1 2022-12-08 08:47:59.000000 thug-6.5/thug/thug.egg-info/dependency_links.txt
+-rw-r--r--   0 buffer    (1000) buffer    (1000)       40 2022-12-08 08:47:59.000000 thug-6.5/thug/thug.egg-info/entry_points.txt
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      486 2022-12-08 08:47:59.000000 thug-6.5/thug/thug.egg-info/requires.txt
+-rw-r--r--   0 buffer    (1000) buffer    (1000)       91 2022-12-08 08:47:59.000000 thug-6.5/thug/thug.egg-info/top_level.txt
+-rw-r--r--   0 buffer    (1000) buffer    (1000)        1 2022-12-07 11:50:03.000000 thug-6.5/thug/thug.egg-info/zip-safe
+-rw-r--r--   0 buffer    (1000) buffer    (1000)    19877 2024-02-22 09:16:59.000000 thug-6.5/thug/thug.py
+drwxr-xr-x   0 buffer    (1000) buffer    (1000)        0 2024-04-11 14:03:15.853458 thug-6.5/thug.egg-info/
+-rw-r--r--   0 buffer    (1000) buffer    (1000)     5613 2024-04-11 14:03:15.000000 thug-6.5/thug.egg-info/PKG-INFO
+-rw-r--r--   0 buffer    (1000) buffer    (1000)    17098 2024-04-11 14:03:15.000000 thug-6.5/thug.egg-info/SOURCES.txt
+-rw-r--r--   0 buffer    (1000) buffer    (1000)        1 2024-04-11 14:03:15.000000 thug-6.5/thug.egg-info/dependency_links.txt
+-rw-r--r--   0 buffer    (1000) buffer    (1000)       40 2024-04-11 14:03:15.000000 thug-6.5/thug.egg-info/entry_points.txt
+-rw-r--r--   0 buffer    (1000) buffer    (1000)      763 2024-04-11 14:03:15.000000 thug-6.5/thug.egg-info/requires.txt
+-rw-r--r--   0 buffer    (1000) buffer    (1000)       10 2024-04-11 14:03:15.000000 thug-6.5/thug.egg-info/top_level.txt
+-rw-r--r--   0 buffer    (1000) buffer    (1000)        1 2024-04-11 14:03:15.000000 thug-6.5/thug.egg-info/zip-safe
```

### Comparing `thug-6.4/LICENSE.txt` & `thug-6.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `thug-6.4/PKG-INFO` & `thug-6.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thug
-Version: 6.4
+Version: 6.5
 Summary: Low-interaction honeyclient Thug
 Author-email: Angelo Dell'Aera <angelo.dellaera@honeynet.org>
 Maintainer-email: Angelo Dell'Aera <angelo.dellaera@honeynet.org>
 License: GPLv2
 Project-URL: homepage, https://github.com/buffer/thug
 Project-URL: documentation, https://thug-honeyclient.readthedocs.io/en/latest/
 Project-URL: bugs, https://github.com/buffer/thug/issues
@@ -29,16 +29,18 @@
 License-File: LICENSE.txt
 Requires-Dist: appdirs==1.4.4
 Requires-Dist: beautifulsoup4==4.12.3
 Requires-Dist: charset-normalizer==3.3.2
 Requires-Dist: cssutils==2.10.2
 Requires-Dist: dhash==1.4
 Requires-Dist: html5lib==1.1
+Requires-Dist: importlib-resources==6.0.1; python_version < "3.9"
 Requires-Dist: lxml==5.2.1
-Requires-Dist: networkx==3.2.1
+Requires-Dist: networkx==3.2.1; python_version < "3.10"
+Requires-Dist: networkx==3.3; python_version > "3.9"
 Requires-Dist: pefile==2023.2.7
 Requires-Dist: pillow==10.3.0
 Requires-Dist: promise==2.3
 Requires-Dist: pylibemu==1.0
 Requires-Dist: pymongo==4.6.3
 Requires-Dist: pysocks==1.7.1
 Requires-Dist: python-magic==0.4.27
@@ -46,15 +48,14 @@
 Requires-Dist: requests==2.31.0
 Requires-Dist: requests-futures==1.0.1
 Requires-Dist: setuptools>=65.5.1
 Requires-Dist: ssdeep==3.4
 Requires-Dist: stpyv8==12.3.219.16
 Requires-Dist: yara-python==4.5.0
 Requires-Dist: zope.interface==6.2
-Requires-Dist: importlib-resources==6.0.1; python_version < "3.9"
 Provides-Extra: elasticsearch
 Requires-Dist: elasticsearch; extra == "elasticsearch"
 Provides-Extra: exploitgraph
 Requires-Dist: pygraphviz; extra == "exploitgraph"
 Provides-Extra: image
 Requires-Dist: imgkit==1.1.0; extra == "image"
 Requires-Dist: pytesseract; extra == "image"
```

### Comparing `thug-6.4/README.rst` & `thug-6.5/README.rst`

 * *Files identical despite different names*

### Comparing `thug-6.4/pyproject.toml` & `thug-6.5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -38,16 +38,18 @@
 dependencies = [
     "appdirs==1.4.4",
     "beautifulsoup4==4.12.3",
     "charset-normalizer==3.3.2",
     "cssutils==2.10.2",
     "dhash==1.4",
     "html5lib==1.1",
+    "importlib-resources==6.0.1; python_version < '3.9'",
     "lxml==5.2.1",
-    "networkx==3.2.1",
+    "networkx==3.2.1; python_version < '3.10'",
+    "networkx==3.3; python_version > '3.9'",
     "pefile==2023.2.7",
     "pillow==10.3.0",
     "promise==2.3",
     "pylibemu==1.0",
     "pymongo==4.6.3",
     "pysocks==1.7.1",
     "python-magic==0.4.27",
@@ -55,17 +57,14 @@
     "requests==2.31.0",
     "requests-futures==1.0.1",
     "setuptools>=65.5.1",
     "ssdeep==3.4",
     "stpyv8==12.3.219.16",
     "yara-python==4.5.0",
     "zope.interface==6.2",
-
-    # Conditional
-    'importlib-resources==6.0.1; python_version < "3.9"',
 ]
 keywords = [
     "honeyclient",
     "low-interaction",
     "client-honeypot",
     "security-tools",
 ]
```

### Comparing `thug-6.4/thug/ActiveX/ActiveX.py` & `thug-6.5/thug/ActiveX/ActiveX.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/CLSID.py` & `thug-6.5/thug/ActiveX/CLSID.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston,
 # MA  02111-1307  USA
 
+import io
+
 from .modules import AcroPDF
 from .modules import AdodbRecordset
 from .modules import AdodbStream
 from .modules import AnswerWorks
 from .modules import AolAmpX
 from .modules import AolICQ
 from .modules import AOLAttack
@@ -90,14 +92,15 @@
 from .modules import SonicWallNetExtenderAddRouteEntry
 from .modules import Spreadsheet
 from .modules import SSReaderPdg2
 from .modules import StormConfig
 from .modules import StormMps
 from .modules import SymantecAppStream
 from .modules import SymantecBackupExec
+from .modules import System
 from .modules import StreamAudioChainCast
 from .modules import Toshiba
 from .modules import UniversalUpload
 from .modules import UUSeeUpdate
 from .modules import VisualStudioDTE80
 from .modules import VLC
 from .modules import VsaIDEDTE
@@ -1284,14 +1287,71 @@
             "Save": SymantecBackupExec.Save,
             "Set_DOWText0": SymantecBackupExec.Set_DOWText0,
             "Set_DOWText6": SymantecBackupExec.Set_DOWText6,
             "Set_MonthText0": SymantecBackupExec.Set_MonthText0,
             "Set_MonthText11": SymantecBackupExec.Set_MonthText11,
         },
     },
+    # System.Collections.ArrayList
+    {
+        "id": (),
+        "name": ("system.collections.arraylist",),
+        "attrs": {
+            "arraylist": [],
+        },
+        "funcattrs": {},
+        "methods": {
+            "Add": System.Collections.ArrayList.Add,
+            "ToArray": System.Collections.ArrayList.ToArray,
+        },
+    },
+    # System.IO.MemoryStream
+    {
+        "id": (),
+        "name": ("system.io.memorystream",),
+        "attrs": {
+            "stream": io.BytesIO(),
+            "Position": 0,
+        },
+        "funcattrs": {},
+        "methods": {
+            "Write": System.IO.MemoryStream.Write,
+        },
+    },
+    # System.Runtime.Serialization.Formatters.Binary.BinaryFormatter
+    {
+        "id": (),
+        "name": ("system.runtime.serialization.formatters.binary.binaryformatter",),
+        "attrs": {},
+        "funcattrs": {},
+        "methods": {
+            "Deserialize_2": System.Runtime.Serialization.Formatters.Binary.BinaryFormatter.Deserialize_2,
+        },
+    },
+    # System.Security.Cryptography.FromBase64Transform
+    {
+        "id": (),
+        "name": ("system.security.cryptography.frombase64transform",),
+        "attrs": {},
+        "funcattrs": {},
+        "methods": {
+            "TransformFinalBlock": System.Security.Cryptography.FromBase64Transform.TransformFinalBlock,
+        },
+    },
+    # System.Text.ASCIIEncoding
+    {
+        "id": (),
+        "name": ("system.text.asciiencoding",),
+        "attrs": {},
+        "funcattrs": {},
+        "methods": {
+            "GetByteCount_2": System.Text.ASCIIEncoding.GetByteCount_2,
+            "GetBytes_4": System.Text.ASCIIEncoding.GetBytes_4,
+        },
+    },
     # StreamAudioChainCast
     {
         "id": ("2253F320-AB68-4A07-917D-4F12D8884A06",),
         "name": ("ccpm.proxymanager.1"),
         "attrs": {},
         "funcattrs": {},
         "methods": {
```

### Comparing `thug-6.4/thug/ActiveX/modules/AcroPDF.py` & `thug-6.5/thug/ActiveX/modules/AcroPDF.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/AdodbRecordset.py` & `thug-6.5/thug/ActiveX/modules/AdodbRecordset.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/AdodbStream.py` & `thug-6.5/thug/ActiveX/modules/AdodbStream.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/AnswerWorks.py` & `thug-6.5/thug/ActiveX/modules/AnswerWorks.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/AolAmpX.py` & `thug-6.5/thug/ActiveX/modules/AolAmpX.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/AolICQ.py` & `thug-6.5/thug/ActiveX/modules/AolICQ.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/BaiduBar.py` & `thug-6.5/thug/ActiveX/modules/BaiduBar.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/CGAgent.py` & `thug-6.5/thug/ActiveX/modules/CGAgent.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/ConnectAndEnterRoom.py` & `thug-6.5/thug/ActiveX/modules/ConnectAndEnterRoom.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/DPClient.py` & `thug-6.5/thug/ActiveX/modules/DPClient.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/DirectShow.py` & `thug-6.5/thug/ActiveX/modules/DirectShow.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/Domino.py` & `thug-6.5/thug/ActiveX/modules/Domino.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/EnjoySAP.py` & `thug-6.5/thug/ActiveX/modules/EnjoySAP.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/FacebookPhotoUploader.py` & `thug-6.5/thug/ActiveX/modules/FacebookPhotoUploader.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/File.py` & `thug-6.5/thug/ActiveX/modules/File.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/Folder.py` & `thug-6.5/thug/ActiveX/modules/Folder.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/GatewayWeblaunch.py` & `thug-6.5/thug/ActiveX/modules/GatewayWeblaunch.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/HPInfo.py` & `thug-6.5/thug/ActiveX/modules/HPInfo.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/IMWebControl.py` & `thug-6.5/thug/ActiveX/modules/IMWebControl.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/JavaDeploymentToolkit.py` & `thug-6.5/thug/ActiveX/modules/JavaDeploymentToolkit.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/JetAudioDownloadFromMusicStore.py` & `thug-6.5/thug/ActiveX/modules/JetAudioDownloadFromMusicStore.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/MSRICHTXT.py` & `thug-6.5/thug/ActiveX/modules/MSRICHTXT.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/MacrovisionFlexNet.py` & `thug-6.5/thug/ActiveX/modules/MacrovisionFlexNet.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/MicrosoftXMLDOM.py` & `thug-6.5/thug/ActiveX/modules/MicrosoftXMLDOM.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/MicrosoftXMLHTTP.py` & `thug-6.5/thug/ActiveX/modules/MicrosoftXMLHTTP.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/NCTAudioFile2.py` & `thug-6.5/thug/ActiveX/modules/NCTAudioFile2.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/NamoInstaller.py` & `thug-6.5/thug/ActiveX/modules/NamoInstaller.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/NeoTracePro.py` & `thug-6.5/thug/ActiveX/modules/NeoTracePro.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/NessusScanCtrl.py` & `thug-6.5/thug/ActiveX/modules/NessusScanCtrl.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/OfficeOCX.py` & `thug-6.5/thug/ActiveX/modules/OfficeOCX.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/OurgameGLWorld.py` & `thug-6.5/thug/ActiveX/modules/OurgameGLWorld.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/PPlayer.py` & `thug-6.5/thug/ActiveX/modules/PPlayer.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/RDSDataSpace.py` & `thug-6.5/thug/ActiveX/modules/RDSDataSpace.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/RealPlayer.py` & `thug-6.5/thug/ActiveX/modules/RealPlayer.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/RegistryPro.py` & `thug-6.5/thug/ActiveX/modules/RegistryPro.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/SSReaderPdg2.py` & `thug-6.5/thug/ActiveX/modules/SSReaderPdg2.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/ScriptingDictionary.py` & `thug-6.5/thug/ActiveX/modules/ScriptingDictionary.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/ScriptingFileSystemObject.py` & `thug-6.5/thug/ActiveX/modules/ScriptingFileSystemObject.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/ShellApplication.py` & `thug-6.5/thug/ActiveX/modules/ShellApplication.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/SinaDLoader.py` & `thug-6.5/thug/ActiveX/modules/SinaDLoader.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/SnapshotViewer.py` & `thug-6.5/thug/ActiveX/modules/SnapshotViewer.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/SonicWallNetExtenderAddRouteEntry.py` & `thug-6.5/thug/ActiveX/modules/SonicWallNetExtenderAddRouteEntry.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/Spreadsheet.py` & `thug-6.5/thug/ActiveX/modules/Spreadsheet.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/StormConfig.py` & `thug-6.5/thug/ActiveX/modules/StormConfig.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/StormMps.py` & `thug-6.5/thug/ActiveX/modules/StormMps.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/SymantecAppStream.py` & `thug-6.5/thug/ActiveX/modules/SymantecAppStream.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/SymantecBackupExec.py` & `thug-6.5/thug/ActiveX/modules/SymantecBackupExec.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/TextStream.py` & `thug-6.5/thug/ActiveX/modules/TextStream.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/Toshiba.py` & `thug-6.5/thug/ActiveX/modules/Toshiba.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/VLC.py` & `thug-6.5/thug/ActiveX/modules/VLC.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/VisualStudioDTE80.py` & `thug-6.5/thug/ActiveX/modules/VisualStudioDTE80.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/WMEncProfileManager.py` & `thug-6.5/thug/ActiveX/modules/WMEncProfileManager.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/WScriptExec.py` & `thug-6.5/thug/ActiveX/modules/WScriptExec.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/WScriptNetwork.py` & `thug-6.5/thug/ActiveX/modules/WScriptNetwork.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/WScriptShell.py` & `thug-6.5/thug/ActiveX/modules/WScriptShell.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/WebViewFolderIcon.py` & `thug-6.5/thug/ActiveX/modules/WebViewFolderIcon.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/WinNTSystemInfo.py` & `thug-6.5/thug/ActiveX/modules/WinNTSystemInfo.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/WinZip.py` & `thug-6.5/thug/ActiveX/modules/WinZip.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/XMLDOMParseError.py` & `thug-6.5/thug/ActiveX/modules/XMLDOMParseError.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/XUpload.py` & `thug-6.5/thug/ActiveX/modules/XUpload.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/YahooJukebox.py` & `thug-6.5/thug/ActiveX/modules/YahooJukebox.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/YahooMessengerYVerInfo.py` & `thug-6.5/thug/ActiveX/modules/YahooMessengerYVerInfo.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/YahooMessengerYwcvwr.py` & `thug-6.5/thug/ActiveX/modules/YahooMessengerYwcvwr.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/ZenturiProgramCheckerAttack.py` & `thug-6.5/thug/ActiveX/modules/ZenturiProgramCheckerAttack.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ActiveX/modules/__init__.py` & `thug-6.5/thug/ActiveX/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/Analysis/awis/AWIS.py` & `thug-6.5/thug/Analysis/awis/AWIS.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/Analysis/context/ContextAnalyzer.py` & `thug-6.5/thug/Analysis/context/ContextAnalyzer.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/Analysis/honeyagent/HoneyAgent.py` & `thug-6.5/thug/Analysis/honeyagent/HoneyAgent.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/Analysis/screenshot/Screenshot.py` & `thug-6.5/thug/Analysis/screenshot/Screenshot.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/Analysis/shellcode/Shellcode.py` & `thug-6.5/thug/Analysis/shellcode/Shellcode.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/Classifier/BaseClassifier.py` & `thug-6.5/thug/Classifier/BaseClassifier.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/Classifier/CookieClassifier.py` & `thug-6.5/thug/Classifier/CookieClassifier.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/Classifier/HTMLClassifier.py` & `thug-6.5/thug/Classifier/HTMLClassifier.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/Classifier/ImageClassifier.py` & `thug-6.5/thug/Classifier/ImageClassifier.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/Classifier/JSClassifier.py` & `thug-6.5/thug/Classifier/JSClassifier.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/Classifier/SampleClassifier.py` & `thug-6.5/thug/Classifier/SampleClassifier.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/Classifier/TextClassifier.py` & `thug-6.5/thug/Classifier/TextClassifier.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/Classifier/URLClassifier.py` & `thug-6.5/thug/Classifier/URLClassifier.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/Classifier/VBSClassifier.py` & `thug-6.5/thug/Classifier/VBSClassifier.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/Alexa.py` & `thug-6.5/thug/DOM/Alexa.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/AsyncPrefetcher.py` & `thug-6.5/thug/DOM/AsyncPrefetcher.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/CCInterpreter.py` & `thug-6.5/thug/DOM/CCInterpreter.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/Chrome.py` & `thug-6.5/thug/DOM/Chrome.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/ClipboardData.py` & `thug-6.5/thug/DOM/ClipboardData.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/Components.py` & `thug-6.5/thug/DOM/Components.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/Console.py` & `thug-6.5/thug/DOM/Console.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/Crypto.py` & `thug-6.5/thug/DOM/Crypto.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/DFT.py` & `thug-6.5/thug/DOM/DFT.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/External.py` & `thug-6.5/thug/DOM/External.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/HTMLInspector.py` & `thug-6.5/thug/DOM/HTMLInspector.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/HTTPSession.py` & `thug-6.5/thug/DOM/HTTPSession.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/HTTPSessionException.py` & `thug-6.5/thug/DOM/HTTPSessionException.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/History.py` & `thug-6.5/thug/DOM/History.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/JSClass.py` & `thug-6.5/thug/DOM/JSClass.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/JSEngine.py` & `thug-6.5/thug/DOM/JSEngine.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/JSInspector.py` & `thug-6.5/thug/DOM/JSInspector.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/JScriptEncode.py` & `thug-6.5/thug/DOM/JScriptEncode.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,132 +3,132 @@
 # This code is derived from the awesome VBE Decoder authored by Didier Stevens
 # and available at https://github.com/DidierStevens/DidierStevensSuite
 
 import re
 
 
 DDECODE = {}
-DDECODE[9] = "\x57\x6E\x7B"
-DDECODE[10] = "\x4A\x4C\x41"
-DDECODE[11] = "\x0B\x0B\x0B"
-DDECODE[12] = "\x0C\x0C\x0C"
-DDECODE[13] = "\x4A\x4C\x41"
-DDECODE[14] = "\x0E\x0E\x0E"
-DDECODE[15] = "\x0F\x0F\x0F"
+DDECODE[9] = "\x57\x6e\x7b"
+DDECODE[10] = "\x4a\x4c\x41"
+DDECODE[11] = "\x0b\x0b\x0b"
+DDECODE[12] = "\x0c\x0c\x0c"
+DDECODE[13] = "\x4a\x4c\x41"
+DDECODE[14] = "\x0e\x0e\x0e"
+DDECODE[15] = "\x0f\x0f\x0f"
 DDECODE[16] = "\x10\x10\x10"
 DDECODE[17] = "\x11\x11\x11"
 DDECODE[18] = "\x12\x12\x12"
 DDECODE[19] = "\x13\x13\x13"
 DDECODE[20] = "\x14\x14\x14"
 DDECODE[21] = "\x15\x15\x15"
 DDECODE[22] = "\x16\x16\x16"
 DDECODE[23] = "\x17\x17\x17"
 DDECODE[24] = "\x18\x18\x18"
 DDECODE[25] = "\x19\x19\x19"
-DDECODE[26] = "\x1A\x1A\x1A"
-DDECODE[27] = "\x1B\x1B\x1B"
-DDECODE[28] = "\x1C\x1C\x1C"
-DDECODE[29] = "\x1D\x1D\x1D"
-DDECODE[30] = "\x1E\x1E\x1E"
-DDECODE[31] = "\x1F\x1F\x1F"
-DDECODE[32] = "\x2E\x2D\x32"
+DDECODE[26] = "\x1a\x1a\x1a"
+DDECODE[27] = "\x1b\x1b\x1b"
+DDECODE[28] = "\x1c\x1c\x1c"
+DDECODE[29] = "\x1d\x1d\x1d"
+DDECODE[30] = "\x1e\x1e\x1e"
+DDECODE[31] = "\x1f\x1f\x1f"
+DDECODE[32] = "\x2e\x2d\x32"
 DDECODE[33] = "\x47\x75\x30"
-DDECODE[34] = "\x7A\x52\x21"
+DDECODE[34] = "\x7a\x52\x21"
 DDECODE[35] = "\x56\x60\x29"
-DDECODE[36] = "\x42\x71\x5B"
-DDECODE[37] = "\x6A\x5E\x38"
-DDECODE[38] = "\x2F\x49\x33"
-DDECODE[39] = "\x26\x5C\x3D"
+DDECODE[36] = "\x42\x71\x5b"
+DDECODE[37] = "\x6a\x5e\x38"
+DDECODE[38] = "\x2f\x49\x33"
+DDECODE[39] = "\x26\x5c\x3d"
 DDECODE[40] = "\x49\x62\x58"
-DDECODE[41] = "\x41\x7D\x3A"
+DDECODE[41] = "\x41\x7d\x3a"
 DDECODE[42] = "\x34\x29\x35"
 DDECODE[43] = "\x32\x36\x65"
-DDECODE[44] = "\x5B\x20\x39"
-DDECODE[45] = "\x76\x7C\x5C"
-DDECODE[46] = "\x72\x7A\x56"
-DDECODE[47] = "\x43\x7F\x73"
-DDECODE[48] = "\x38\x6B\x66"
-DDECODE[49] = "\x39\x63\x4E"
+DDECODE[44] = "\x5b\x20\x39"
+DDECODE[45] = "\x76\x7c\x5c"
+DDECODE[46] = "\x72\x7a\x56"
+DDECODE[47] = "\x43\x7f\x73"
+DDECODE[48] = "\x38\x6b\x66"
+DDECODE[49] = "\x39\x63\x4e"
 DDECODE[50] = "\x70\x33\x45"
-DDECODE[51] = "\x45\x2B\x6B"
+DDECODE[51] = "\x45\x2b\x6b"
 DDECODE[52] = "\x68\x68\x62"
 DDECODE[53] = "\x71\x51\x59"
-DDECODE[54] = "\x4F\x66\x78"
-DDECODE[55] = "\x09\x76\x5E"
-DDECODE[56] = "\x62\x31\x7D"
-DDECODE[57] = "\x44\x64\x4A"
-DDECODE[58] = "\x23\x54\x6D"
+DDECODE[54] = "\x4f\x66\x78"
+DDECODE[55] = "\x09\x76\x5e"
+DDECODE[56] = "\x62\x31\x7d"
+DDECODE[57] = "\x44\x64\x4a"
+DDECODE[58] = "\x23\x54\x6d"
 DDECODE[59] = "\x75\x43\x71"
-DDECODE[60] = "\x4A\x4C\x41"
-DDECODE[61] = "\x7E\x3A\x60"
-DDECODE[62] = "\x4A\x4C\x41"
-DDECODE[63] = "\x5E\x7E\x53"
-DDECODE[64] = "\x40\x4C\x40"
+DDECODE[60] = "\x4a\x4c\x41"
+DDECODE[61] = "\x7e\x3a\x60"
+DDECODE[62] = "\x4a\x4c\x41"
+DDECODE[63] = "\x5e\x7e\x53"
+DDECODE[64] = "\x40\x4c\x40"
 DDECODE[65] = "\x77\x45\x42"
-DDECODE[66] = "\x4A\x2C\x27"
-DDECODE[67] = "\x61\x2A\x48"
-DDECODE[68] = "\x5D\x74\x72"
+DDECODE[66] = "\x4a\x2c\x27"
+DDECODE[67] = "\x61\x2a\x48"
+DDECODE[68] = "\x5d\x74\x72"
 DDECODE[69] = "\x22\x27\x75"
-DDECODE[70] = "\x4B\x37\x31"
-DDECODE[71] = "\x6F\x44\x37"
-DDECODE[72] = "\x4E\x79\x4D"
-DDECODE[73] = "\x3B\x59\x52"
-DDECODE[74] = "\x4C\x2F\x22"
-DDECODE[75] = "\x50\x6F\x54"
-DDECODE[76] = "\x67\x26\x6A"
-DDECODE[77] = "\x2A\x72\x47"
-DDECODE[78] = "\x7D\x6A\x64"
-DDECODE[79] = "\x74\x39\x2D"
-DDECODE[80] = "\x54\x7B\x20"
-DDECODE[81] = "\x2B\x3F\x7F"
-DDECODE[82] = "\x2D\x38\x2E"
-DDECODE[83] = "\x2C\x77\x4C"
-DDECODE[84] = "\x30\x67\x5D"
-DDECODE[85] = "\x6E\x53\x7E"
-DDECODE[86] = "\x6B\x47\x6C"
-DDECODE[87] = "\x66\x34\x6F"
+DDECODE[70] = "\x4b\x37\x31"
+DDECODE[71] = "\x6f\x44\x37"
+DDECODE[72] = "\x4e\x79\x4d"
+DDECODE[73] = "\x3b\x59\x52"
+DDECODE[74] = "\x4c\x2f\x22"
+DDECODE[75] = "\x50\x6f\x54"
+DDECODE[76] = "\x67\x26\x6a"
+DDECODE[77] = "\x2a\x72\x47"
+DDECODE[78] = "\x7d\x6a\x64"
+DDECODE[79] = "\x74\x39\x2d"
+DDECODE[80] = "\x54\x7b\x20"
+DDECODE[81] = "\x2b\x3f\x7f"
+DDECODE[82] = "\x2d\x38\x2e"
+DDECODE[83] = "\x2c\x77\x4c"
+DDECODE[84] = "\x30\x67\x5d"
+DDECODE[85] = "\x6e\x53\x7e"
+DDECODE[86] = "\x6b\x47\x6c"
+DDECODE[87] = "\x66\x34\x6f"
 DDECODE[88] = "\x35\x78\x79"
-DDECODE[89] = "\x25\x5D\x74"
+DDECODE[89] = "\x25\x5d\x74"
 DDECODE[90] = "\x21\x30\x43"
 DDECODE[91] = "\x64\x23\x26"
-DDECODE[92] = "\x4D\x5A\x76"
-DDECODE[93] = "\x52\x5B\x25"
-DDECODE[94] = "\x63\x6C\x24"
-DDECODE[95] = "\x3F\x48\x2B"
-DDECODE[96] = "\x7B\x55\x28"
+DDECODE[92] = "\x4d\x5a\x76"
+DDECODE[93] = "\x52\x5b\x25"
+DDECODE[94] = "\x63\x6c\x24"
+DDECODE[95] = "\x3f\x48\x2b"
+DDECODE[96] = "\x7b\x55\x28"
 DDECODE[97] = "\x78\x70\x23"
 DDECODE[98] = "\x29\x69\x41"
-DDECODE[99] = "\x28\x2E\x34"
-DDECODE[100] = "\x73\x4C\x09"
-DDECODE[101] = "\x59\x21\x2A"
+DDECODE[99] = "\x28\x2e\x34"
+DDECODE[100] = "\x73\x4c\x09"
+DDECODE[101] = "\x59\x21\x2a"
 DDECODE[102] = "\x33\x24\x44"
-DDECODE[103] = "\x7F\x4E\x3F"
-DDECODE[104] = "\x6D\x50\x77"
-DDECODE[105] = "\x55\x09\x3B"
+DDECODE[103] = "\x7f\x4e\x3f"
+DDECODE[104] = "\x6d\x50\x77"
+DDECODE[105] = "\x55\x09\x3b"
 DDECODE[106] = "\x53\x56\x55"
-DDECODE[107] = "\x7C\x73\x69"
-DDECODE[108] = "\x3A\x35\x61"
-DDECODE[109] = "\x5F\x61\x63"
-DDECODE[110] = "\x65\x4B\x50"
+DDECODE[107] = "\x7c\x73\x69"
+DDECODE[108] = "\x3a\x35\x61"
+DDECODE[109] = "\x5f\x61\x63"
+DDECODE[110] = "\x65\x4b\x50"
 DDECODE[111] = "\x46\x58\x67"
-DDECODE[112] = "\x58\x3B\x51"
+DDECODE[112] = "\x58\x3b\x51"
 DDECODE[113] = "\x31\x57\x49"
-DDECODE[114] = "\x69\x22\x4F"
-DDECODE[115] = "\x6C\x6D\x46"
-DDECODE[116] = "\x5A\x4D\x68"
-DDECODE[117] = "\x48\x25\x7C"
+DDECODE[114] = "\x69\x22\x4f"
+DDECODE[115] = "\x6c\x6d\x46"
+DDECODE[116] = "\x5a\x4d\x68"
+DDECODE[117] = "\x48\x25\x7c"
 DDECODE[118] = "\x27\x28\x36"
-DDECODE[119] = "\x5C\x46\x70"
-DDECODE[120] = "\x3D\x4A\x6E"
-DDECODE[121] = "\x24\x32\x7A"
-DDECODE[122] = "\x79\x41\x2F"
-DDECODE[123] = "\x37\x3D\x5F"
-DDECODE[124] = "\x60\x5F\x4B"
-DDECODE[125] = "\x51\x4F\x5A"
-DDECODE[126] = "\x20\x42\x2C"
+DDECODE[119] = "\x5c\x46\x70"
+DDECODE[120] = "\x3d\x4a\x6e"
+DDECODE[121] = "\x24\x32\x7a"
+DDECODE[122] = "\x79\x41\x2f"
+DDECODE[123] = "\x37\x3d\x5f"
+DDECODE[124] = "\x60\x5f\x4b"
+DDECODE[125] = "\x51\x4f\x5a"
+DDECODE[126] = "\x20\x42\x2c"
 DDECODE[127] = "\x36\x65\x57"
 
 DCOMBINATION = {}
 DCOMBINATION[0] = 0
 DCOMBINATION[1] = 1
 DCOMBINATION[2] = 2
 DCOMBINATION[3] = 0
```

### Comparing `thug-6.4/thug/DOM/LocalStorage.py` & `thug-6.5/thug/DOM/LocalStorage.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/Location.py` & `thug-6.5/thug/DOM/Location.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/MIMEHandler.py` & `thug-6.5/thug/DOM/MIMEHandler.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/Map.py` & `thug-6.5/thug/DOM/Map.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/MimeType.py` & `thug-6.5/thug/DOM/MimeType.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/MimeTypes.py` & `thug-6.5/thug/DOM/MimeTypes.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/MozConnection.py` & `thug-6.5/thug/DOM/MozConnection.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/Navigator.py` & `thug-6.5/thug/DOM/Navigator.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/Personality.py` & `thug-6.5/thug/DOM/Personality.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/Plugin.py` & `thug-6.5/thug/DOM/Plugin.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/Plugins.py` & `thug-6.5/thug/DOM/Plugins.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/SchemeHandler.py` & `thug-6.5/thug/DOM/SchemeHandler.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/Screen.py` & `thug-6.5/thug/DOM/Screen.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/SessionStorage.py` & `thug-6.5/thug/DOM/SessionStorage.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/Sidebar.py` & `thug-6.5/thug/DOM/Sidebar.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/Storage.py` & `thug-6.5/thug/DOM/Storage.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/UserProfile.py` & `thug-6.5/thug/DOM/UserProfile.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/Utils.py` & `thug-6.5/thug/DOM/Utils.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/Core/Attr.py` & `thug-6.5/thug/DOM/W3C/Core/Attr.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/Core/CharacterData.py` & `thug-6.5/thug/DOM/W3C/Core/CharacterData.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/Core/ClassList.py` & `thug-6.5/thug/DOM/W3C/Core/ClassList.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/Core/Comment.py` & `thug-6.5/thug/DOM/W3C/Core/Comment.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/Core/DOMException.py` & `thug-6.5/thug/DOM/W3C/Core/DOMException.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/Core/DOMImplementation.py` & `thug-6.5/thug/DOM/W3C/Core/DOMImplementation.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/Core/Document.py` & `thug-6.5/thug/DOM/W3C/Core/Document.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/Core/DocumentFragment.py` & `thug-6.5/thug/DOM/W3C/Core/DocumentFragment.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/Core/DocumentType.py` & `thug-6.5/thug/DOM/W3C/Core/DocumentType.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/Core/Element.py` & `thug-6.5/thug/DOM/W3C/Core/Element.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/Core/NamedNodeMap.py` & `thug-6.5/thug/DOM/W3C/Core/NamedNodeMap.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/Core/Node.py` & `thug-6.5/thug/DOM/W3C/Core/Node.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/Core/NodeList.py` & `thug-6.5/thug/DOM/W3C/Core/NodeList.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/Core/Text.py` & `thug-6.5/thug/DOM/W3C/Core/Text.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/Core/__init__.py` & `thug-6.5/thug/DOM/W3C/Core/__init__.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/DOMTokenList.py` & `thug-6.5/thug/DOM/W3C/DOMTokenList.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/Events/DocumentEvent.py` & `thug-6.5/thug/DOM/W3C/Events/DocumentEvent.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/Events/Event.py` & `thug-6.5/thug/DOM/W3C/Events/Event.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/Events/EventTarget.py` & `thug-6.5/thug/DOM/W3C/Events/EventTarget.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/Events/MessageEvent.py` & `thug-6.5/thug/DOM/W3C/Events/MessageEvent.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/Events/MouseEvent.py` & `thug-6.5/thug/DOM/W3C/Events/MouseEvent.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/Events/MutationEvent.py` & `thug-6.5/thug/DOM/W3C/Events/MutationEvent.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/Events/StorageEvent.py` & `thug-6.5/thug/DOM/W3C/Events/StorageEvent.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/Events/UIEvent.py` & `thug-6.5/thug/DOM/W3C/Events/UIEvent.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/Events/__init__.py` & `thug-6.5/thug/DOM/W3C/Events/__init__.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/File/Blob.py` & `thug-6.5/thug/DOM/W3C/File/Blob.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/File/File.py` & `thug-6.5/thug/DOM/W3C/File/File.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/HTML/Dataset.py` & `thug-6.5/thug/DOM/W3C/HTML/Dataset.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/HTML/HTMLAnchorElement.py` & `thug-6.5/thug/DOM/W3C/HTML/HTMLAnchorElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/HTML/HTMLAppletElement.py` & `thug-6.5/thug/DOM/W3C/HTML/HTMLAppletElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/HTML/HTMLBodyElement.py` & `thug-6.5/thug/DOM/W3C/HTML/HTMLBodyElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/HTML/HTMLButtonElement.py` & `thug-6.5/thug/DOM/W3C/HTML/HTMLButtonElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/HTML/HTMLCollection.py` & `thug-6.5/thug/DOM/W3C/HTML/HTMLCollection.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/HTML/HTMLDocument.py` & `thug-6.5/thug/DOM/W3C/HTML/HTMLDocument.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/HTML/HTMLDocumentCompatibleInfo.py` & `thug-6.5/thug/DOM/W3C/HTML/HTMLDocumentCompatibleInfo.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/HTML/HTMLElement.py` & `thug-6.5/thug/DOM/W3C/HTML/HTMLElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/HTML/HTMLFormElement.py` & `thug-6.5/thug/DOM/W3C/HTML/HTMLFormElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/HTML/HTMLFrameElement.py` & `thug-6.5/thug/DOM/W3C/HTML/HTMLFrameElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/HTML/HTMLIFrameElement.py` & `thug-6.5/thug/DOM/W3C/HTML/HTMLIFrameElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/HTML/HTMLImageElement.py` & `thug-6.5/thug/DOM/W3C/HTML/HTMLImageElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/HTML/HTMLInputElement.py` & `thug-6.5/thug/DOM/W3C/HTML/HTMLInputElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/HTML/HTMLLinkElement.py` & `thug-6.5/thug/DOM/W3C/HTML/HTMLLinkElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/HTML/HTMLMediaElement.py` & `thug-6.5/thug/DOM/W3C/HTML/HTMLMediaElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/HTML/HTMLMetaElement.py` & `thug-6.5/thug/DOM/W3C/HTML/HTMLMetaElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/HTML/HTMLObjectElement.py` & `thug-6.5/thug/DOM/W3C/HTML/HTMLObjectElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/HTML/HTMLOptionElement.py` & `thug-6.5/thug/DOM/W3C/HTML/HTMLOptionElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/HTML/HTMLScriptElement.py` & `thug-6.5/thug/DOM/W3C/HTML/HTMLScriptElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/HTML/HTMLSelectElement.py` & `thug-6.5/thug/DOM/W3C/HTML/HTMLSelectElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/HTML/HTMLTableCellElement.py` & `thug-6.5/thug/DOM/W3C/HTML/HTMLTableCellElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/HTML/HTMLTableElement.py` & `thug-6.5/thug/DOM/W3C/HTML/HTMLTableElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/HTML/HTMLTableRowElement.py` & `thug-6.5/thug/DOM/W3C/HTML/HTMLTableRowElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/HTML/HTMLTableSectionElement.py` & `thug-6.5/thug/DOM/W3C/HTML/HTMLTableSectionElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/HTML/HTMLTextAreaElement.py` & `thug-6.5/thug/DOM/W3C/HTML/HTMLTextAreaElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/HTML/HTMLVideoElement.py` & `thug-6.5/thug/DOM/W3C/HTML/HTMLVideoElement.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/HTML/TAnimateColor.py` & `thug-6.5/thug/DOM/W3C/HTML/TAnimateColor.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/HTML/TimeRanges.py` & `thug-6.5/thug/DOM/W3C/HTML/TimeRanges.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/HTML/__init__.py` & `thug-6.5/thug/DOM/W3C/HTML/__init__.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/HTML/text_property.py` & `thug-6.5/thug/DOM/W3C/HTML/text_property.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/Style/CSS/CSSStyleDeclaration.py` & `thug-6.5/thug/DOM/W3C/Style/CSS/CSSStyleDeclaration.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/URL/URL.py` & `thug-6.5/thug/DOM/W3C/URL/URL.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/W3C/URL/URLSearchParams.py` & `thug-6.5/thug/DOM/W3C/URL/URLSearchParams.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/WebStore.py` & `thug-6.5/thug/DOM/WebStore.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/Window.py` & `thug-6.5/thug/DOM/Window.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/DOM/w3c_bindings.py` & `thug-6.5/thug/DOM/w3c_bindings.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/Encoding/Encoding.py` & `thug-6.5/thug/Encoding/Encoding.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/Java/System.py` & `thug-6.5/thug/Java/System.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/Java/java.py` & `thug-6.5/thug/Java/java.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/Java/lang.py` & `thug-6.5/thug/Java/lang.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/Logging/BaseLogging.py` & `thug-6.5/thug/Logging/BaseLogging.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/Logging/Features.py` & `thug-6.5/thug/Logging/Features.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/Logging/LoggingModules.py` & `thug-6.5/thug/Logging/LoggingModules.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/Logging/SampleLogging.py` & `thug-6.5/thug/Logging/SampleLogging.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/Logging/ThugLogging.py` & `thug-6.5/thug/Logging/ThugLogging.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/Logging/modules/ElasticSearch.py` & `thug-6.5/thug/Logging/modules/ElasticSearch.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/Logging/modules/ExploitGraph.py` & `thug-6.5/thug/Logging/modules/ExploitGraph.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/Logging/modules/JSON.py` & `thug-6.5/thug/Logging/modules/JSON.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/Logging/modules/Mapper.py` & `thug-6.5/thug/Logging/modules/Mapper.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/Logging/modules/MongoDB.py` & `thug-6.5/thug/Logging/modules/MongoDB.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/Magic/Magic.py` & `thug-6.5/thug/Magic/Magic.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/OS/Windows.py` & `thug-6.5/thug/OS/Windows.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/Plugins/IPlugin.py` & `thug-6.5/thug/Plugins/IPlugin.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/Plugins/ThugPlugins.py` & `thug-6.5/thug/Plugins/ThugPlugins.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/Plugins/plugins/POST-TestPlugin-999/Handler.py` & `thug-6.5/thug/Plugins/plugins/POST-TestPlugin-999/Handler.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/Plugins/plugins/PRE-TestPlugin-999/Handler.py` & `thug-6.5/thug/Plugins/plugins/PRE-TestPlugin-999/Handler.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ThugAPI/IThugAPI.py` & `thug-6.5/thug/ThugAPI/IThugAPI.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ThugAPI/OpaqueFilter.py` & `thug-6.5/thug/ThugAPI/OpaqueFilter.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ThugAPI/ThugAPI.py` & `thug-6.5/thug/ThugAPI/ThugAPI.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ThugAPI/ThugOpts.py` & `thug-6.5/thug/ThugAPI/ThugOpts.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ThugAPI/ThugVulnModules.py` & `thug-6.5/thug/ThugAPI/ThugVulnModules.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/ThugAPI/Watchdog.py` & `thug-6.5/thug/ThugAPI/Watchdog.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/WebTracking/Cookies.py` & `thug-6.5/thug/WebTracking/Cookies.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/WebTracking/WebStorage.py` & `thug-6.5/thug/WebTracking/WebStorage.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/WebTracking/WebTracking.py` & `thug-6.5/thug/WebTracking/WebTracking.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/__init__.py` & `thug-6.5/thug/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import importlib.resources
 
 import appdirs
 
-__version__ = "6.4"
+__version__ = "6.5"
 __jsengine__ = ""
 __jsengine_version__ = ""
 
 __global_configuration_path__ = "/etc/thug"
 __user_configuration_path__ = f"{appdirs.user_config_dir()}/thug"
 __package_configuration_path__ = os.path.join(importlib.resources.files("thug"), "conf")
 __configuration_path__ = __package_configuration_path__
```

### Comparing `thug-6.4/thug/conf/personalities/galaxy2chrome18.json` & `thug-6.5/thug/conf/personalities/galaxy2chrome18.json`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/conf/personalities/galaxy2chrome25.json` & `thug-6.5/thug/conf/personalities/galaxy2chrome25.json`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/conf/personalities/galaxy2chrome29.json` & `thug-6.5/thug/conf/personalities/galaxy2chrome29.json`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/conf/personalities/ipadchrome33.json` & `thug-6.5/thug/conf/personalities/ipadchrome33.json`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/conf/personalities/ipadchrome35.json` & `thug-6.5/thug/conf/personalities/ipadchrome35.json`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/conf/personalities/ipadchrome37.json` & `thug-6.5/thug/conf/personalities/ipadchrome37.json`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/conf/personalities/ipadchrome38.json` & `thug-6.5/thug/conf/personalities/ipadchrome38.json`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/conf/personalities/ipadchrome39.json` & `thug-6.5/thug/conf/personalities/ipadchrome39.json`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/conf/personalities/ipadchrome45.json` & `thug-6.5/thug/conf/personalities/ipadchrome45.json`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/conf/personalities/ipadchrome46.json` & `thug-6.5/thug/conf/personalities/ipadchrome46.json`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/conf/personalities/ipadchrome47.json` & `thug-6.5/thug/conf/personalities/ipadchrome47.json`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/conf/personalities/ipadsafari7.json` & `thug-6.5/thug/conf/personalities/ipadsafari7.json`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/conf/personalities/ipadsafari8.json` & `thug-6.5/thug/conf/personalities/ipadsafari8.json`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/conf/personalities/ipadsafari9.json` & `thug-6.5/thug/conf/personalities/ipadsafari9.json`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/conf/personalities/linuxchrome26.json` & `thug-6.5/thug/conf/personalities/linuxchrome26.json`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/conf/personalities/linuxchrome30.json` & `thug-6.5/thug/conf/personalities/linuxchrome30.json`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/conf/personalities/linuxchrome44.json` & `thug-6.5/thug/conf/personalities/linuxchrome44.json`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/conf/personalities/linuxchrome54.json` & `thug-6.5/thug/conf/personalities/linuxchrome54.json`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/conf/personalities/linuxchrome98.json` & `thug-6.5/thug/conf/personalities/linuxchrome98.json`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/conf/personalities/linuxfirefox19.json` & `thug-6.5/thug/conf/personalities/linuxfirefox19.json`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/conf/personalities/linuxfirefox40.json` & `thug-6.5/thug/conf/personalities/linuxfirefox40.json`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/conf/personalities/nexuschrome18.json` & `thug-6.5/thug/conf/personalities/nexuschrome18.json`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/conf/personalities/osx10chrome19.json` & `thug-6.5/thug/conf/personalities/osx10chrome19.json`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/conf/personalities/osx10chrome80.json` & `thug-6.5/thug/conf/personalities/osx10chrome80.json`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/conf/personalities/osx10chrome97.json` & `thug-6.5/thug/conf/personalities/osx10chrome97.json`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/conf/personalities/osx10safari5.json` & `thug-6.5/thug/conf/personalities/osx10safari5.json`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/conf/personalities/osx11safari14.json` & `thug-6.5/thug/conf/personalities/osx11safari14.json`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/conf/personalities/win10edge20.json.review` & `thug-6.5/thug/conf/personalities/win10edge20.json.review`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/conf/personalities/win10ie110.json` & `thug-6.5/thug/conf/personalities/win10ie110.json`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/conf/personalities/win2kie60.json` & `thug-6.5/thug/conf/personalities/win2kie60.json`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/conf/personalities/win2kie80.json` & `thug-6.5/thug/conf/personalities/win2kie80.json`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/conf/personalities/win7chrome20.json` & `thug-6.5/thug/conf/personalities/win7chrome20.json`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/conf/personalities/win7chrome40.json` & `thug-6.5/thug/conf/personalities/win7chrome40.json`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/conf/personalities/win7chrome45.json` & `thug-6.5/thug/conf/personalities/win7chrome45.json`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/conf/personalities/win7chrome49.json` & `thug-6.5/thug/conf/personalities/win7chrome49.json`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/conf/personalities/win7firefox3.json` & `thug-6.5/thug/conf/personalities/win7firefox3.json`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/conf/personalities/win7ie100.json` & `thug-6.5/thug/conf/personalities/win7ie100.json`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/conf/personalities/win7ie80.json` & `thug-6.5/thug/conf/personalities/win7ie80.json`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/conf/personalities/win7ie90.json` & `thug-6.5/thug/conf/personalities/win7ie90.json`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/conf/personalities/win7safari5.json` & `thug-6.5/thug/conf/personalities/win7safari5.json`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/conf/personalities/winxpchrome20.json` & `thug-6.5/thug/conf/personalities/winxpchrome20.json`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/conf/personalities/winxpfirefox12.json` & `thug-6.5/thug/conf/personalities/winxpfirefox12.json`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/conf/personalities/winxpie60.json` & `thug-6.5/thug/conf/personalities/winxpie60.json`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/conf/personalities/winxpie61.json` & `thug-6.5/thug/conf/personalities/winxpie61.json`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/conf/personalities/winxpie70.json` & `thug-6.5/thug/conf/personalities/winxpie70.json`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/conf/personalities/winxpie80.json` & `thug-6.5/thug/conf/personalities/winxpie80.json`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/conf/personalities/winxpsafari5.json` & `thug-6.5/thug/conf/personalities/winxpsafari5.json`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/conf/rules/urlclassifier/blackhole.yar` & `thug-6.5/thug/conf/rules/urlclassifier/blackhole.yar`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/conf/rules/urlclassifier/crimeboss.yar` & `thug-6.5/thug/conf/rules/urlclassifier/crimeboss.yar`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/conf/rules/urlclassifier/critxpack.yar` & `thug-6.5/thug/conf/rules/urlclassifier/critxpack.yar`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/conf/rules/urlclassifier/fiesta.yar` & `thug-6.5/thug/conf/rules/urlclassifier/fiesta.yar`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/conf/rules/urlclassifier/g01pack.yar` & `thug-6.5/thug/conf/rules/urlclassifier/g01pack.yar`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/conf/rules/urlclassifier/neutrino.yar` & `thug-6.5/thug/conf/rules/urlclassifier/neutrino.yar`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/conf/rules/urlclassifier/nuclear.yar` & `thug-6.5/thug/conf/rules/urlclassifier/nuclear.yar`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/conf/rules/urlclassifier/popads.yar` & `thug-6.5/thug/conf/rules/urlclassifier/popads.yar`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/conf/rules/urlclassifier/redkit.yar` & `thug-6.5/thug/conf/rules/urlclassifier/redkit.yar`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/conf/rules/urlclassifier/styx.yar` & `thug-6.5/thug/conf/rules/urlclassifier/styx.yar`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/conf/rules/urlclassifier/sweetorange.yar` & `thug-6.5/thug/conf/rules/urlclassifier/sweetorange.yar`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/conf/scripts/atob.js` & `thug-6.5/thug/conf/scripts/atob.js`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/conf/scripts/btoa.js` & `thug-6.5/thug/conf/scripts/btoa.js`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/conf/scripts/thug.js` & `thug-6.5/thug/conf/scripts/thug.js`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug/thug.py` & `thug-6.5/thug/thug.py`

 * *Files identical despite different names*

### Comparing `thug-6.4/thug.egg-info/PKG-INFO` & `thug-6.5/thug.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thug
-Version: 6.4
+Version: 6.5
 Summary: Low-interaction honeyclient Thug
 Author-email: Angelo Dell'Aera <angelo.dellaera@honeynet.org>
 Maintainer-email: Angelo Dell'Aera <angelo.dellaera@honeynet.org>
 License: GPLv2
 Project-URL: homepage, https://github.com/buffer/thug
 Project-URL: documentation, https://thug-honeyclient.readthedocs.io/en/latest/
 Project-URL: bugs, https://github.com/buffer/thug/issues
@@ -29,16 +29,18 @@
 License-File: LICENSE.txt
 Requires-Dist: appdirs==1.4.4
 Requires-Dist: beautifulsoup4==4.12.3
 Requires-Dist: charset-normalizer==3.3.2
 Requires-Dist: cssutils==2.10.2
 Requires-Dist: dhash==1.4
 Requires-Dist: html5lib==1.1
+Requires-Dist: importlib-resources==6.0.1; python_version < "3.9"
 Requires-Dist: lxml==5.2.1
-Requires-Dist: networkx==3.2.1
+Requires-Dist: networkx==3.2.1; python_version < "3.10"
+Requires-Dist: networkx==3.3; python_version > "3.9"
 Requires-Dist: pefile==2023.2.7
 Requires-Dist: pillow==10.3.0
 Requires-Dist: promise==2.3
 Requires-Dist: pylibemu==1.0
 Requires-Dist: pymongo==4.6.3
 Requires-Dist: pysocks==1.7.1
 Requires-Dist: python-magic==0.4.27
@@ -46,15 +48,14 @@
 Requires-Dist: requests==2.31.0
 Requires-Dist: requests-futures==1.0.1
 Requires-Dist: setuptools>=65.5.1
 Requires-Dist: ssdeep==3.4
 Requires-Dist: stpyv8==12.3.219.16
 Requires-Dist: yara-python==4.5.0
 Requires-Dist: zope.interface==6.2
-Requires-Dist: importlib-resources==6.0.1; python_version < "3.9"
 Provides-Extra: elasticsearch
 Requires-Dist: elasticsearch; extra == "elasticsearch"
 Provides-Extra: exploitgraph
 Requires-Dist: pygraphviz; extra == "exploitgraph"
 Provides-Extra: image
 Requires-Dist: imgkit==1.1.0; extra == "image"
 Requires-Dist: pytesseract; extra == "image"
```

### Comparing `thug-6.4/thug.egg-info/SOURCES.txt` & `thug-6.5/thug.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -118,14 +118,31 @@
 thug/ActiveX/modules/XUpload.py
 thug/ActiveX/modules/YahooJukebox.py
 thug/ActiveX/modules/YahooMessengerCyft.py
 thug/ActiveX/modules/YahooMessengerYVerInfo.py
 thug/ActiveX/modules/YahooMessengerYwcvwr.py
 thug/ActiveX/modules/ZenturiProgramCheckerAttack.py
 thug/ActiveX/modules/__init__.py
+thug/ActiveX/modules/System/__init__.py
+thug/ActiveX/modules/System/Collections/ArrayList.py
+thug/ActiveX/modules/System/Collections/__init__.py
+thug/ActiveX/modules/System/IO/MemoryStream.py
+thug/ActiveX/modules/System/IO/__init__.py
+thug/ActiveX/modules/System/Runtime/Activator.py
+thug/ActiveX/modules/System/Runtime/Delegate.py
+thug/ActiveX/modules/System/Runtime/__init__.py
+thug/ActiveX/modules/System/Runtime/Serialization/__init__.py
+thug/ActiveX/modules/System/Runtime/Serialization/Formatters/__init__.py
+thug/ActiveX/modules/System/Runtime/Serialization/Formatters/Binary/BinaryFormatter.py
+thug/ActiveX/modules/System/Runtime/Serialization/Formatters/Binary/__init__.py
+thug/ActiveX/modules/System/Security/__init__.py
+thug/ActiveX/modules/System/Security/Cryptography/FromBase64Transform.py
+thug/ActiveX/modules/System/Security/Cryptography/__init__.py
+thug/ActiveX/modules/System/Text/ASCIIEncoding.py
+thug/ActiveX/modules/System/Text/__init__.py
 thug/Analysis/__init__.py
 thug/Analysis/awis/AWIS.py
 thug/Analysis/awis/__init__.py
 thug/Analysis/context/ContextAnalyzer.py
 thug/Analysis/context/__init__.py
 thug/Analysis/favicon/Favicon.py
 thug/Analysis/favicon/__init__.py
@@ -454,8 +471,15 @@
 thug/conf/scripts/atob.js
 thug/conf/scripts/btoa.js
 thug/conf/scripts/date.js
 thug/conf/scripts/eval.js
 thug/conf/scripts/message-event.js
 thug/conf/scripts/storage.js
 thug/conf/scripts/thug.js
-thug/conf/scripts/write.js
+thug/conf/scripts/write.js
+thug/thug.egg-info/PKG-INFO
+thug/thug.egg-info/SOURCES.txt
+thug/thug.egg-info/dependency_links.txt
+thug/thug.egg-info/entry_points.txt
+thug/thug.egg-info/requires.txt
+thug/thug.egg-info/top_level.txt
+thug/thug.egg-info/zip-safe
```

### Comparing `thug-6.4/thug.egg-info/requires.txt` & `thug-6.5/thug.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 appdirs==1.4.4
 beautifulsoup4==4.12.3
 charset-normalizer==3.3.2
 cssutils==2.10.2
 dhash==1.4
 html5lib==1.1
 lxml==5.2.1
-networkx==3.2.1
 pefile==2023.2.7
 pillow==10.3.0
 promise==2.3
 pylibemu==1.0
 pymongo==4.6.3
 pysocks==1.7.1
 python-magic==0.4.27
@@ -18,17 +17,23 @@
 requests-futures==1.0.1
 setuptools>=65.5.1
 ssdeep==3.4
 stpyv8==12.3.219.16
 yara-python==4.5.0
 zope.interface==6.2
 
+[:python_version < "3.10"]
+networkx==3.2.1
+
 [:python_version < "3.9"]
 importlib-resources==6.0.1
 
+[:python_version > "3.9"]
+networkx==3.3
+
 [elasticsearch]
 elasticsearch
 
 [exploitgraph]
 pygraphviz
 
 [image]
```

