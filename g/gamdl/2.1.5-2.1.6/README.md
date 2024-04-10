# Comparing `tmp/gamdl-2.1.5.tar.gz` & `tmp/gamdl-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gamdl-2.1.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gamdl-2.1.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gamdl-2.1.5.tar` & `gamdl-2.1.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0       35 2024-04-09 16:19:14.480419 gamdl-2.1.5/.github/FUNDING.yml
--rw-r--r--   0        0        0     1137 2024-04-09 16:19:14.480419 gamdl-2.1.5/.github/workflows/main.yml
--rw-r--r--   0        0        0       79 2024-04-09 16:19:14.480419 gamdl-2.1.5/.gitignore
--rw-r--r--   0        0        0    11240 2024-04-09 16:19:14.480419 gamdl-2.1.5/README.md
--rw-r--r--   0        0        0       22 2024-04-09 16:19:14.480419 gamdl-2.1.5/gamdl/__init__.py
--rw-r--r--   0        0        0       30 2024-04-09 16:19:14.480419 gamdl-2.1.5/gamdl/__main__.py
--rw-r--r--   0        0        0     7930 2024-04-09 16:19:14.480419 gamdl-2.1.5/gamdl/apple_music_api.py
--rw-r--r--   0        0        0    26303 2024-04-09 16:19:14.480419 gamdl-2.1.5/gamdl/cli.py
--rw-r--r--   0        0        0     5544 2024-04-09 16:19:14.480419 gamdl-2.1.5/gamdl/constants.py
--rw-r--r--   0        0        0    12606 2024-04-09 16:19:14.480419 gamdl-2.1.5/gamdl/downloader.py
--rw-r--r--   0        0        0    10392 2024-04-09 16:19:14.480419 gamdl-2.1.5/gamdl/downloader_music_video.py
--rw-r--r--   0        0        0     2152 2024-04-09 16:19:14.480419 gamdl-2.1.5/gamdl/downloader_post.py
--rw-r--r--   0        0        0    13802 2024-04-09 16:19:14.480419 gamdl-2.1.5/gamdl/downloader_song.py
--rw-r--r--   0        0        0     3691 2024-04-09 16:19:14.480419 gamdl-2.1.5/gamdl/downloader_song_legacy.py
--rw-r--r--   0        0        0      801 2024-04-09 16:19:14.480419 gamdl-2.1.5/gamdl/enums.py
--rw-r--r--   0        0        0     4015 2024-04-09 16:19:14.480419 gamdl-2.1.5/gamdl/hardcoded_wvd.py
--rw-r--r--   0        0        0     2418 2024-04-09 16:19:14.480419 gamdl-2.1.5/gamdl/itunes_api.py
--rw-r--r--   0        0        0      369 2024-04-09 16:19:14.480419 gamdl-2.1.5/gamdl/models.py
--rw-r--r--   0        0        0      560 2024-04-09 16:19:14.480419 gamdl-2.1.5/pyproject.toml
--rw-r--r--   0        0        0       54 2024-04-09 16:19:14.480419 gamdl-2.1.5/requirements.txt
--rw-r--r--   0        0        0    11715 1970-01-01 00:00:00.000000 gamdl-2.1.5/PKG-INFO
+-rw-r--r--   0        0        0       17 2024-04-10 22:05:31.703859 gamdl-2.1.6/.github/FUNDING.yml
+-rw-r--r--   0        0        0     1137 2024-04-10 22:05:31.703859 gamdl-2.1.6/.github/workflows/main.yml
+-rw-r--r--   0        0        0       79 2024-04-10 22:05:31.703859 gamdl-2.1.6/.gitignore
+-rw-r--r--   0        0        0    11844 2024-04-10 22:05:31.703859 gamdl-2.1.6/README.md
+-rw-r--r--   0        0        0       22 2024-04-10 22:05:31.703859 gamdl-2.1.6/gamdl/__init__.py
+-rw-r--r--   0        0        0       30 2024-04-10 22:05:31.703859 gamdl-2.1.6/gamdl/__main__.py
+-rw-r--r--   0        0        0     7930 2024-04-10 22:05:31.703859 gamdl-2.1.6/gamdl/apple_music_api.py
+-rw-r--r--   0        0        0    26576 2024-04-10 22:05:31.703859 gamdl-2.1.6/gamdl/cli.py
+-rw-r--r--   0        0        0     5580 2024-04-10 22:05:31.707859 gamdl-2.1.6/gamdl/constants.py
+-rw-r--r--   0        0        0    12691 2024-04-10 22:05:31.707859 gamdl-2.1.6/gamdl/downloader.py
+-rw-r--r--   0        0        0    10392 2024-04-10 22:05:31.707859 gamdl-2.1.6/gamdl/downloader_music_video.py
+-rw-r--r--   0        0        0     2254 2024-04-10 22:05:31.707859 gamdl-2.1.6/gamdl/downloader_post.py
+-rw-r--r--   0        0        0    13976 2024-04-10 22:05:31.707859 gamdl-2.1.6/gamdl/downloader_song.py
+-rw-r--r--   0        0        0     3865 2024-04-10 22:05:31.707859 gamdl-2.1.6/gamdl/downloader_song_legacy.py
+-rw-r--r--   0        0        0      817 2024-04-10 22:05:31.707859 gamdl-2.1.6/gamdl/enums.py
+-rw-r--r--   0        0        0     4015 2024-04-10 22:05:31.707859 gamdl-2.1.6/gamdl/hardcoded_wvd.py
+-rw-r--r--   0        0        0     2418 2024-04-10 22:05:31.707859 gamdl-2.1.6/gamdl/itunes_api.py
+-rw-r--r--   0        0        0      369 2024-04-10 22:05:31.707859 gamdl-2.1.6/gamdl/models.py
+-rw-r--r--   0        0        0      560 2024-04-10 22:05:31.707859 gamdl-2.1.6/pyproject.toml
+-rw-r--r--   0        0        0       54 2024-04-10 22:05:31.707859 gamdl-2.1.6/requirements.txt
+-rw-r--r--   0        0        0    12319 1970-01-01 00:00:00.000000 gamdl-2.1.6/PKG-INFO
```

### Comparing `gamdl-2.1.5/.github/workflows/main.yml` & `gamdl-2.1.6/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.5/README.md` & `gamdl-2.1.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -39,51 +39,53 @@
 * Download an album
     ```bash
     gamdl "https://music.apple.com/us/album/whenever-you-need-somebody-2022-remaster/1626265761"
     ```
 
 ## Configuration
 You can configure gamdl by using the command line arguments or the config file. The config file is created automatically when you run gamdl for the first time at `~/.gamdl/config.json` on Linux and `%USERPROFILE%\.gamdl\config.json` on Windows. Config file values can be overridden using command line arguments.
-| Command line argument / Config file key                         | Description                                                        | Default value                                |
-| --------------------------------------------------------------- | ------------------------------------------------------------------ | -------------------------------------------- |
-| `--disable-music-video-skip` / `disable_music_video_skip`       | Don't skip downloading music videos in albums/playlists.           | `false`                                      |
-| `--save-cover`, `-s` / `save_cover`                             | Save cover as a separate file.                                     | `false`                                      |
-| `--overwrite` / `overwrite`                                     | Overwrite existing files.                                          | `false`                                      |
-| `--read-urls-as-txt`, `-r` / -                                  | Interpret URLs as paths to text files containing URLs.             | `false`                                      |
-| `--synced-lyrics-only` / `synced_lyrics_only`                   | Download only the synced lyrics.                                   | `false`                                      |
-| `--no-synced-lyrics` / `no_synced_lyrics`                       | Don't download the synced lyrics.                                  | `false`                                      |
-| `--config-path` / -                                             | Path to config file.                                               | `<home>/.spotify-web-downloader/config.json` |
-| `--log-level` / `log_level`                                     | Log level.                                                         | `INFO`                                       |
-| `--print-exceptions` / `print_exceptions`                       | Print exceptions.                                                  | `false`                                      |
-| `--cookies-path`, `-c` / `cookies_path`                         | Path to .txt cookies file.                                         | `./cookies.txt`                              |
-| `--output-path`, `-o` / `output_path`                           | Path to output directory.                                          | `./Apple Music`                              |
-| `--temp-path` / `temp_path`                                     | Path to temporary directory.                                       | `./temp`                                     |
-| `--wvd-path` / `wvd_path`                                       | Path to .wvd file.                                                 | `null`                                       |
-| `--nm3u8dlre-path` / `nm3u8dlre_path`                           | Path to N_m3u8DL-RE binary.                                        | `N_m3u8dl-RE`                                |
-| `--mp4decrypt-path` / `mp4decrypt_path`                         | Path to mp4decrypt binary.                                         | `mp4decrypt`                                 |
-| `--ffmpeg-path` / `ffmpeg_path`                                 | Path to FFmpeg binary.                                             | `ffmpeg`                                     |
-| `--mp4box-path` / `mp4box_path`                                 | Path to MP4Box binary.                                             | `MP4Box`                                     |
-| `--download-mode` / `download_mode`                             | Download mode.                                                     | `ytdlp`                                      |
-| `--remux-mode` / `remux_mode`                                   | Remux mode.                                                        | `ffmpeg`                                     |
-| `--cover-format` / `cover_format`                               | Cover format.                                                      | `jpg`                                        |
-| `--template-folder-album` / `template_folder_album`             | Template folder for tracks that are part of an album.              | `{album_artist}/{album}`                     |
-| `--template-folder-compilation` / `template_folder_compilation` | Template folder for tracks that are part of a compilation album.   | `Compilations/{album}`                       |
-| `--template-file-single-disc` / `template_file_single_disc`     | Template file for the tracks that are part of a single-disc album. | `{track:02d} {title}`                        |
-| `--template-file-multi-disc` / `template_file_multi_disc`       | Template file for the tracks that are part of a multi-disc album.  | `{disc}-{track:02d} {title}`                 |
-| `--template-folder-no-album` / `template_folder_no_album`       | Template folder for the tracks that are not part of an album.      | `{artist}/Unknown Album`                     |
-| `--template-file-no-album` / `template_file_no_album`           | Template file for the tracks that are not part of an album.        | `{title}`                                    |
-| `--template-date` / `template_date`                             | Date tag template.                                                 | `%Y-%m-%dT%H:%M:%SZ`                         |
-| `--exclude-tags` / `exclude_tags`                               | Comma-separated tags to exclude.                                   | `null`                                       |
-| `--cover-size` / `cover_size`                                   | Cover size.                                                        | `1200`                                       |
-| `--truncate` / `truncate`                                       | Maximum length of the file/folder names.                           | `40`                                         |
-| `--codec-song` / `codec_song`                                   | Song codec.                                                        | `aac-legacy`                                 |
-| `--synced-lyrics-format` / `synced_lyrics_format`               | Synced lyrics format.                                              | `lrc`                                        |
-| `--codec-music-video` / `codec_music_video`                     | Music video codec.                                                 | `h264-best`                                  |
-| `--quality-post` / `quality_post`                               | Post video quality.                                                | `best`                                       |
-| `--no-config-file`, `-n` / -                                    | Do not use a config file.                                          | `false`                                      |
+| Command line argument / Config file key                         | Description                                                                  | Default value                                |
+| --------------------------------------------------------------- | ---------------------------------------------------------------------------- | -------------------------------------------- |
+| `--disable-music-video-skip` / `disable_music_video_skip`       | Don't skip downloading music videos in albums/playlists.                     | `false`                                      |
+| `--save-cover`, `-s` / `save_cover`                             | Save cover as a separate file.                                               | `false`                                      |
+| `--overwrite` / `overwrite`                                     | Overwrite existing files.                                                    | `false`                                      |
+| `--read-urls-as-txt`, `-r` / -                                  | Interpret URLs as paths to text files containing URLs.                       | `false`                                      |
+| `--synced-lyrics-only` / `synced_lyrics_only`                   | Download only the synced lyrics.                                             | `false`                                      |
+| `--no-synced-lyrics` / `no_synced_lyrics`                       | Don't download the synced lyrics.                                            | `false`                                      |
+| `--config-path` / -                                             | Path to config file.                                                         | `<home>/.spotify-web-downloader/config.json` |
+| `--log-level` / `log_level`                                     | Log level.                                                                   | `INFO`                                       |
+| `--print-exceptions` / `print_exceptions`                       | Print exceptions.                                                            | `false`                                      |
+| `--cookies-path`, `-c` / `cookies_path`                         | Path to .txt cookies file.                                                   | `./cookies.txt`                              |
+| `--language`, `-l` / `language`                                 | Metadata language as an ISO-2A language code (don't always work for videos). | `en-US`                                      |
+| `--output-path`, `-o` / `output_path`                           | Path to output directory.                                                    | `./Apple Music`                              |
+| `--temp-path` / `temp_path`                                     | Path to temporary directory.                                                 | `./temp`                                     |
+| `--wvd-path` / `wvd_path`                                       | Path to .wvd file.                                                           | `null`                                       |
+| `--nm3u8dlre-path` / `nm3u8dlre_path`                           | Path to N_m3u8DL-RE binary.                                                  | `N_m3u8dl-RE`                                |
+| `--mp4decrypt-path` / `mp4decrypt_path`                         | Path to mp4decrypt binary.                                                   | `mp4decrypt`                                 |
+| `--ffmpeg-path` / `ffmpeg_path`                                 | Path to FFmpeg binary.                                                       | `ffmpeg`                                     |
+| `--mp4box-path` / `mp4box_path`                                 | Path to MP4Box binary.                                                       | `MP4Box`                                     |
+| `--download-mode` / `download_mode`                             | Download mode.                                                               | `ytdlp`                                      |
+| `--remux-mode` / `remux_mode`                                   | Remux mode.                                                                  | `ffmpeg`                                     |
+| `--cover-format` / `cover_format`                               | Cover format.                                                                | `jpg`                                        |
+| `--template-folder-album` / `template_folder_album`             | Template folder for tracks that are part of an album.                        | `{album_artist}/{album}`                     |
+| `--template-folder-compilation` / `template_folder_compilation` | Template folder for tracks that are part of a compilation album.             | `Compilations/{album}`                       |
+| `--template-file-single-disc` / `template_file_single_disc`     | Template file for the tracks that are part of a single-disc album.           | `{track:02d} {title}`                        |
+| `--template-file-multi-disc` / `template_file_multi_disc`       | Template file for the tracks that are part of a multi-disc album.            | `{disc}-{track:02d} {title}`                 |
+| `--template-folder-no-album` / `template_folder_no_album`       | Template folder for the tracks that are not part of an album.                | `{artist}/Unknown Album`                     |
+| `--template-file-no-album` / `template_file_no_album`           | Template file for the tracks that are not part of an album.                  | `{title}`                                    |
+| `--template-date` / `template_date`                             | Date tag template.                                                           | `%Y-%m-%dT%H:%M:%SZ`                         |
+| `--exclude-tags` / `exclude_tags`                               | Comma-separated tags to exclude.                                             | `null`                                       |
+| `--cover-size` / `cover_size`                                   | Cover size.                                                                  | `1200`                                       |
+| `--truncate` / `truncate`                                       | Maximum length of the file/folder names.                                     | `40`                                         |
+| `--codec-song` / `codec_song`                                   | Song codec.                                                                  | `aac-legacy`                                 |
+| `--synced-lyrics-format` / `synced_lyrics_format`               | Synced lyrics format.                                                        | `lrc`                                        |
+| `--codec-music-video` / `codec_music_video`                     | Music video codec.                                                           | `h264-best`                                  |
+| `--quality-post` / `quality_post`                               | Post video quality.                                                          | `best`                                       |
+| `--no-config-file`, `-n` / -                                    | Do not use a config file.                                                    | `false`                                      |
+
 
 ### Tags variables
 The following variables can be used in the template folders/files and/or in the `exclude_tags` list:
 * `album`
 * `album_artist`
 * `album_id`
 * `album_sort`
@@ -138,18 +140,19 @@
 * `aac-he-legacy`
 * `aac`
 * `aac-he`
 * `aac-binaural`
 * `aac-downmix`
 * `aac-he-binaural`
 * `aac-he-downmix`
-* `alac`
 * `atmos`
+* `ac3`
+* `alac`
 * `ask`
-    * When using this option, the script will ask you which **non-legacy** codec to use.
+    * When using this option, the script will ask you which **non-legacy** codec to use that is available for the song.
 
 **Support for non-legacy codecs are not guaranteed, as most of the songs cannot be downloaded when using non-legacy codecs.**
 
 ### Music videos codecs
 The following codecs are available:
 * `h264-best` (with AAC 256kbps, up to 1080p)
 * `h265-best` (With AAC 256kpbs, up to 2160p)
```

### Comparing `gamdl-2.1.5/gamdl/apple_music_api.py` & `gamdl-2.1.6/gamdl/apple_music_api.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.5/gamdl/cli.py` & `gamdl-2.1.6/gamdl/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,14 +128,21 @@
 @click.option(
     "--cookies-path",
     "-c",
     type=Path,
     default=apple_music_api_sig.parameters["cookies_path"].default,
     help="Path to .txt cookies file.",
 )
+@click.option(
+    "--language",
+    "-l",
+    type=str,
+    default=apple_music_api_sig.parameters["language"].default,
+    help="Metadata language as an ISO-2A language code (don't always work for videos).",
+)
 # Downloader specific options
 @click.option(
     "--output-path",
     "-o",
     type=Path,
     default=downloader_sig.parameters["output_path"].default,
     help="Path to output directory.",
@@ -297,14 +304,15 @@
     read_urls_as_txt: bool,
     synced_lyrics_only: bool,
     no_synced_lyrics: bool,
     config_path: Path,
     log_level: str,
     print_exceptions: bool,
     cookies_path: Path,
+    language: str,
     output_path: Path,
     temp_path: Path,
     wvd_path: Path,
     nm3u8dlre_path: str,
     mp4decrypt_path: str,
     ffmpeg_path: str,
     mp4box_path: str,
@@ -330,15 +338,18 @@
     logging.basicConfig(
         format="[%(levelname)-8s %(asctime)s] %(message)s",
         datefmt="%H:%M:%S",
     )
     logger = logging.getLogger(__name__)
     logger.setLevel(log_level)
     logger.debug("Starting downloader")
-    apple_music_api = AppleMusicApi(cookies_path)
+    apple_music_api = AppleMusicApi(
+        cookies_path,
+        language=language,
+    )
     itunes_api = ItunesApi(
         apple_music_api.storefront,
         apple_music_api.language,
     )
     downloader = Downloader(
         apple_music_api,
         itunes_api,
```

### Comparing `gamdl-2.1.5/gamdl/constants.py` & `gamdl-2.1.6/gamdl/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,16 +187,17 @@
 SONG_CODEC_REGEX_MAP = {
     SongCodec.AAC: r"audio-stereo-\d+",
     SongCodec.AAC_HE: r"audio-HE-stereo-\d+",
     SongCodec.AAC_BINAURAL: r"audio-stereo-\d+-binaural",
     SongCodec.AAC_DOWNMIX: r"audio-stereo-\d+-downmix",
     SongCodec.AAC_HE_BINAURAL: r"audio-HE-stereo-\d+-binaural",
     SongCodec.AAC_HE_DOWNMIX: r"audio-HE-stereo-\d+-downmix",
-    SongCodec.ALAC: r"audio-alac-.*",
     SongCodec.ATMOS: r"audio-atmos-.*",
+    SongCodec.AC3: r"audio-ac3-.*",
+    SongCodec.ALAC: r"audio-alac-.*",
 }
 
 MUSIC_VIDEO_CODEC_MAP = {
     MusicVideoCodec.H264_BEST: "avc1",
     MusicVideoCodec.H265_BEST: "hvc1",
 }
```

### Comparing `gamdl-2.1.5/gamdl/downloader.py` & `gamdl-2.1.6/gamdl/downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         template_file_multi_disc: str = "{disc}-{track:02d} {title}",
         template_folder_no_album: str = "{artist}/Unknown Album",
         template_file_no_album: str = "{title}",
         template_date: str = "%Y-%m-%dT%H:%M:%SZ",
         exclude_tags: str = None,
         cover_size: int = 1200,
         truncate: int = 40,
-        no_progress: bool = False,
+        silent: bool = False,
     ):
         self.apple_music_api = apple_music_api
         self.itunes_api = itunes_api
         self.output_path = output_path
         self.temp_path = temp_path
         self.wvd_path = wvd_path
         self.nm3u8dlre_path = nm3u8dlre_path
@@ -68,18 +68,19 @@
         self.template_file_multi_disc = template_file_multi_disc
         self.template_folder_no_album = template_folder_no_album
         self.template_file_no_album = template_file_no_album
         self.template_date = template_date
         self.exclude_tags = exclude_tags
         self.cover_size = cover_size
         self.truncate = truncate
-        self.no_progress = no_progress
+        self.silent = silent
         self._set_binaries_path_full()
         self._set_exclude_tags_list()
         self._set_truncate()
+        self._set_subprocess_additional_args()
 
     def _set_binaries_path_full(self):
         self.nm3u8dlre_path_full = shutil.which(self.nm3u8dlre_path)
         self.ffmpeg_path_full = shutil.which(self.ffmpeg_path)
         self.mp4box_path_full = shutil.which(self.mp4box_path)
         self.mp4decrypt_path_full = shutil.which(self.mp4decrypt_path)
 
@@ -89,14 +90,23 @@
             if self.exclude_tags is not None
             else []
         )
 
     def _set_truncate(self):
         self.truncate = None if self.truncate < 4 else self.truncate
 
+    def _set_subprocess_additional_args(self):
+        if self.silent:
+            self.subprocess_additional_args = {
+                "stdout": subprocess.DEVNULL,
+                "stderr": subprocess.DEVNULL,
+            }
+        else:
+            self.subprocess_additional_args = {}
+
     def set_cdm(self):
         if self.wvd_path:
             self.cdm = Cdm.from_device(Device.load(self.wvd_path))
         else:
             self.cdm = Cdm.from_device(Device.loads(HARDCODED_WVD))
 
     def get_url_info(self, url: str) -> UrlInfo:
@@ -179,27 +189,20 @@
             {
                 "quiet": True,
                 "no_warnings": True,
                 "outtmpl": str(path),
                 "allow_unplayable_formats": True,
                 "fixup": "never",
                 "allowed_extractors": ["generic"],
-                "noprogress": self.no_progress,
+                "noprogress": self.silent,
             }
         ) as ydl:
             ydl.download(stream_url)
 
     def download_nm3u8dlre(self, path: Path, stream_url: str):
-        if self.no_progress:
-            subprocess_additional_args = {
-                "stdout": subprocess.DEVNULL,
-                "stderr": subprocess.DEVNULL,
-            }
-        else:
-            subprocess_additional_args = {}
         path.parent.mkdir(parents=True, exist_ok=True)
         subprocess.run(
             [
                 self.nm3u8dlre_path_full,
                 stream_url,
                 "--binary-merge",
                 "--no-log",
@@ -211,15 +214,15 @@
                 path.stem,
                 "--save-dir",
                 path.parent,
                 "--tmp-dir",
                 path.parent,
             ],
             check=True,
-            **subprocess_additional_args,
+            **self.subprocess_additional_args,
         )
 
     def get_sanitized_string(self, dirty_string: str, is_folder: bool) -> str:
         dirty_string = re.sub(self.ILLEGAL_CHARACTERS_REGEX, "_", dirty_string)
         if is_folder:
             dirty_string = dirty_string[: self.truncate]
             if dirty_string.endswith("."):
```

### Comparing `gamdl-2.1.5/gamdl/downloader_music_video.py` & `gamdl-2.1.6/gamdl/downloader_music_video.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.5/gamdl/downloader_post.py` & `gamdl-2.1.6/gamdl/downloader_post.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,17 +42,20 @@
             [index, quality]
             for index, quality in enumerate(
                 qualities,
                 start=1,
             )
         ]
         print(tabulate(table))
-        choice = (
-            click.prompt("Choose a quality", type=click.IntRange(1, len(table))) - 1
-        )
+        try:
+            choice = (
+                click.prompt("Choose a quality", type=click.IntRange(1, len(table))) - 1
+            )
+        except click.exceptions.Abort:
+            raise KeyboardInterrupt()
         return metadata["attributes"]["assetTokens"][qualities[choice]]
 
     def get_stream_url(self, metadata: dict) -> str:
         if self.quality == PostQuality.BEST:
             stream_url = self.get_stream_url_best(metadata)
         elif self.quality == PostQuality.ASK:
             stream_url = self.get_stream_url_from_user(metadata)
```

### Comparing `gamdl-2.1.5/gamdl/downloader_song.py` & `gamdl-2.1.6/gamdl/downloader_song.py`

 * *Files 2% similar despite different names*

```diff
@@ -296,14 +296,15 @@
                 "--key",
                 f"00000000000000000000000000000001:{decryption_key}",
                 "--key",
                 f"00000000000000000000000000000000:{self.DEFAULT_DECRYPTION_KEY}",
                 decrypted_path,
             ],
             check=True,
+            **self.downloader.subprocess_additional_args,
         )
 
     def remux(self, decrypted_path: Path, remuxed_path: Path, codec: str):
         if self.downloader.remux_mode == RemuxMode.MP4BOX:
             self.remux_mp4box(decrypted_path, remuxed_path)
         elif self.downloader.remux_mode == RemuxMode.FFMPEG:
             self.remux_ffmpeg(decrypted_path, remuxed_path, codec)
@@ -317,14 +318,15 @@
                 decrypted_path,
                 "-itags",
                 "artist=placeholder",
                 "-new",
                 remuxed_path,
             ],
             check=True,
+            **self.downloader.subprocess_additional_args,
         )
 
     def remux_ffmpeg(
         self,
         decrypted_path: Path,
         remuxed_path: Path,
         codec: str,
@@ -346,14 +348,15 @@
                 "-f",
                 "mp4" if use_mp4_format else "ipod",
                 "-movflags",
                 "+faststart",
                 remuxed_path,
             ],
             check=True,
+            **self.downloader.subprocess_additional_args,
         )
 
     def get_lyrics_synced_path(self, final_path: Path) -> Path:
         return final_path.with_suffix(
             SYNCED_LYRICS_FILE_EXTENSION_MAP[self.synced_lyrics_format]
         )
```

### Comparing `gamdl-2.1.5/gamdl/downloader_song_legacy.py` & `gamdl-2.1.6/gamdl/downloader_song_legacy.py`

 * *Files 18% similar despite different names*

```diff
@@ -58,14 +58,15 @@
                 self.downloader.mp4decrypt_path_full,
                 encrypted_path,
                 "--key",
                 f"1:{decryption_key}",
                 decrypted_path,
             ],
             check=True,
+            **self.downloader.subprocess_additional_args,
         )
 
     def remux_mp4box(self, decrypted_path: Path, remuxed_path: Path) -> None:
         subprocess.run(
             [
                 self.downloader.mp4box_path_full,
                 "-quiet",
@@ -73,14 +74,15 @@
                 decrypted_path,
                 "-itags",
                 "artist=placeholder",
                 "-new",
                 remuxed_path,
             ],
             check=True,
+            **self.downloader.subprocess_additional_args,
         )
 
     def remux_ffmpeg(
         self,
         decryption_key: str,
         encrypted_path: Path,
         remuxed_path: Path,
@@ -98,14 +100,15 @@
                 "-c",
                 "copy",
                 "-movflags",
                 "+faststart",
                 remuxed_path,
             ],
             check=True,
+            **self.downloader.subprocess_additional_args,
         )
 
     def remux(
         self,
         encrypted_path: Path,
         decrypted_path: Path,
         remuxed_path: Path,
```

### Comparing `gamdl-2.1.5/gamdl/enums.py` & `gamdl-2.1.6/gamdl/enums.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,16 +16,17 @@
     AAC_HE_LEGACY = "aac-he-legacy"
     AAC = "aac"
     AAC_HE = "aac-he"
     AAC_BINAURAL = "aac-binaural"
     AAC_DOWNMIX = "aac-downmix"
     AAC_HE_BINAURAL = "aac-he-binaural"
     AAC_HE_DOWNMIX = "aac-he-downmix"
-    ALAC = "alac"
     ATMOS = "atmos"
+    AC3 = "ac3"
+    ALAC = "alac"
     ASK = "ask"
 
 
 class SyncedLyricsFormat(Enum):
     LRC = "lrc"
     SRT = "srt"
     TTML = "ttml"
```

### Comparing `gamdl-2.1.5/gamdl/hardcoded_wvd.py` & `gamdl-2.1.6/gamdl/hardcoded_wvd.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.5/gamdl/itunes_api.py` & `gamdl-2.1.6/gamdl/itunes_api.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.5/pyproject.toml` & `gamdl-2.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.5/PKG-INFO` & `gamdl-2.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gamdl
-Version: 2.1.5
+Version: 2.1.6
 Summary: Download Apple Music songs/music videos/albums/playlists
 Author: glomatico
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: ciso8601
 Requires-Dist: click
 Requires-Dist: m3u8
@@ -56,51 +56,53 @@
 * Download an album
     ```bash
     gamdl "https://music.apple.com/us/album/whenever-you-need-somebody-2022-remaster/1626265761"
     ```
 
 ## Configuration
 You can configure gamdl by using the command line arguments or the config file. The config file is created automatically when you run gamdl for the first time at `~/.gamdl/config.json` on Linux and `%USERPROFILE%\.gamdl\config.json` on Windows. Config file values can be overridden using command line arguments.
-| Command line argument / Config file key                         | Description                                                        | Default value                                |
-| --------------------------------------------------------------- | ------------------------------------------------------------------ | -------------------------------------------- |
-| `--disable-music-video-skip` / `disable_music_video_skip`       | Don't skip downloading music videos in albums/playlists.           | `false`                                      |
-| `--save-cover`, `-s` / `save_cover`                             | Save cover as a separate file.                                     | `false`                                      |
-| `--overwrite` / `overwrite`                                     | Overwrite existing files.                                          | `false`                                      |
-| `--read-urls-as-txt`, `-r` / -                                  | Interpret URLs as paths to text files containing URLs.             | `false`                                      |
-| `--synced-lyrics-only` / `synced_lyrics_only`                   | Download only the synced lyrics.                                   | `false`                                      |
-| `--no-synced-lyrics` / `no_synced_lyrics`                       | Don't download the synced lyrics.                                  | `false`                                      |
-| `--config-path` / -                                             | Path to config file.                                               | `<home>/.spotify-web-downloader/config.json` |
-| `--log-level` / `log_level`                                     | Log level.                                                         | `INFO`                                       |
-| `--print-exceptions` / `print_exceptions`                       | Print exceptions.                                                  | `false`                                      |
-| `--cookies-path`, `-c` / `cookies_path`                         | Path to .txt cookies file.                                         | `./cookies.txt`                              |
-| `--output-path`, `-o` / `output_path`                           | Path to output directory.                                          | `./Apple Music`                              |
-| `--temp-path` / `temp_path`                                     | Path to temporary directory.                                       | `./temp`                                     |
-| `--wvd-path` / `wvd_path`                                       | Path to .wvd file.                                                 | `null`                                       |
-| `--nm3u8dlre-path` / `nm3u8dlre_path`                           | Path to N_m3u8DL-RE binary.                                        | `N_m3u8dl-RE`                                |
-| `--mp4decrypt-path` / `mp4decrypt_path`                         | Path to mp4decrypt binary.                                         | `mp4decrypt`                                 |
-| `--ffmpeg-path` / `ffmpeg_path`                                 | Path to FFmpeg binary.                                             | `ffmpeg`                                     |
-| `--mp4box-path` / `mp4box_path`                                 | Path to MP4Box binary.                                             | `MP4Box`                                     |
-| `--download-mode` / `download_mode`                             | Download mode.                                                     | `ytdlp`                                      |
-| `--remux-mode` / `remux_mode`                                   | Remux mode.                                                        | `ffmpeg`                                     |
-| `--cover-format` / `cover_format`                               | Cover format.                                                      | `jpg`                                        |
-| `--template-folder-album` / `template_folder_album`             | Template folder for tracks that are part of an album.              | `{album_artist}/{album}`                     |
-| `--template-folder-compilation` / `template_folder_compilation` | Template folder for tracks that are part of a compilation album.   | `Compilations/{album}`                       |
-| `--template-file-single-disc` / `template_file_single_disc`     | Template file for the tracks that are part of a single-disc album. | `{track:02d} {title}`                        |
-| `--template-file-multi-disc` / `template_file_multi_disc`       | Template file for the tracks that are part of a multi-disc album.  | `{disc}-{track:02d} {title}`                 |
-| `--template-folder-no-album` / `template_folder_no_album`       | Template folder for the tracks that are not part of an album.      | `{artist}/Unknown Album`                     |
-| `--template-file-no-album` / `template_file_no_album`           | Template file for the tracks that are not part of an album.        | `{title}`                                    |
-| `--template-date` / `template_date`                             | Date tag template.                                                 | `%Y-%m-%dT%H:%M:%SZ`                         |
-| `--exclude-tags` / `exclude_tags`                               | Comma-separated tags to exclude.                                   | `null`                                       |
-| `--cover-size` / `cover_size`                                   | Cover size.                                                        | `1200`                                       |
-| `--truncate` / `truncate`                                       | Maximum length of the file/folder names.                           | `40`                                         |
-| `--codec-song` / `codec_song`                                   | Song codec.                                                        | `aac-legacy`                                 |
-| `--synced-lyrics-format` / `synced_lyrics_format`               | Synced lyrics format.                                              | `lrc`                                        |
-| `--codec-music-video` / `codec_music_video`                     | Music video codec.                                                 | `h264-best`                                  |
-| `--quality-post` / `quality_post`                               | Post video quality.                                                | `best`                                       |
-| `--no-config-file`, `-n` / -                                    | Do not use a config file.                                          | `false`                                      |
+| Command line argument / Config file key                         | Description                                                                  | Default value                                |
+| --------------------------------------------------------------- | ---------------------------------------------------------------------------- | -------------------------------------------- |
+| `--disable-music-video-skip` / `disable_music_video_skip`       | Don't skip downloading music videos in albums/playlists.                     | `false`                                      |
+| `--save-cover`, `-s` / `save_cover`                             | Save cover as a separate file.                                               | `false`                                      |
+| `--overwrite` / `overwrite`                                     | Overwrite existing files.                                                    | `false`                                      |
+| `--read-urls-as-txt`, `-r` / -                                  | Interpret URLs as paths to text files containing URLs.                       | `false`                                      |
+| `--synced-lyrics-only` / `synced_lyrics_only`                   | Download only the synced lyrics.                                             | `false`                                      |
+| `--no-synced-lyrics` / `no_synced_lyrics`                       | Don't download the synced lyrics.                                            | `false`                                      |
+| `--config-path` / -                                             | Path to config file.                                                         | `<home>/.spotify-web-downloader/config.json` |
+| `--log-level` / `log_level`                                     | Log level.                                                                   | `INFO`                                       |
+| `--print-exceptions` / `print_exceptions`                       | Print exceptions.                                                            | `false`                                      |
+| `--cookies-path`, `-c` / `cookies_path`                         | Path to .txt cookies file.                                                   | `./cookies.txt`                              |
+| `--language`, `-l` / `language`                                 | Metadata language as an ISO-2A language code (don't always work for videos). | `en-US`                                      |
+| `--output-path`, `-o` / `output_path`                           | Path to output directory.                                                    | `./Apple Music`                              |
+| `--temp-path` / `temp_path`                                     | Path to temporary directory.                                                 | `./temp`                                     |
+| `--wvd-path` / `wvd_path`                                       | Path to .wvd file.                                                           | `null`                                       |
+| `--nm3u8dlre-path` / `nm3u8dlre_path`                           | Path to N_m3u8DL-RE binary.                                                  | `N_m3u8dl-RE`                                |
+| `--mp4decrypt-path` / `mp4decrypt_path`                         | Path to mp4decrypt binary.                                                   | `mp4decrypt`                                 |
+| `--ffmpeg-path` / `ffmpeg_path`                                 | Path to FFmpeg binary.                                                       | `ffmpeg`                                     |
+| `--mp4box-path` / `mp4box_path`                                 | Path to MP4Box binary.                                                       | `MP4Box`                                     |
+| `--download-mode` / `download_mode`                             | Download mode.                                                               | `ytdlp`                                      |
+| `--remux-mode` / `remux_mode`                                   | Remux mode.                                                                  | `ffmpeg`                                     |
+| `--cover-format` / `cover_format`                               | Cover format.                                                                | `jpg`                                        |
+| `--template-folder-album` / `template_folder_album`             | Template folder for tracks that are part of an album.                        | `{album_artist}/{album}`                     |
+| `--template-folder-compilation` / `template_folder_compilation` | Template folder for tracks that are part of a compilation album.             | `Compilations/{album}`                       |
+| `--template-file-single-disc` / `template_file_single_disc`     | Template file for the tracks that are part of a single-disc album.           | `{track:02d} {title}`                        |
+| `--template-file-multi-disc` / `template_file_multi_disc`       | Template file for the tracks that are part of a multi-disc album.            | `{disc}-{track:02d} {title}`                 |
+| `--template-folder-no-album` / `template_folder_no_album`       | Template folder for the tracks that are not part of an album.                | `{artist}/Unknown Album`                     |
+| `--template-file-no-album` / `template_file_no_album`           | Template file for the tracks that are not part of an album.                  | `{title}`                                    |
+| `--template-date` / `template_date`                             | Date tag template.                                                           | `%Y-%m-%dT%H:%M:%SZ`                         |
+| `--exclude-tags` / `exclude_tags`                               | Comma-separated tags to exclude.                                             | `null`                                       |
+| `--cover-size` / `cover_size`                                   | Cover size.                                                                  | `1200`                                       |
+| `--truncate` / `truncate`                                       | Maximum length of the file/folder names.                                     | `40`                                         |
+| `--codec-song` / `codec_song`                                   | Song codec.                                                                  | `aac-legacy`                                 |
+| `--synced-lyrics-format` / `synced_lyrics_format`               | Synced lyrics format.                                                        | `lrc`                                        |
+| `--codec-music-video` / `codec_music_video`                     | Music video codec.                                                           | `h264-best`                                  |
+| `--quality-post` / `quality_post`                               | Post video quality.                                                          | `best`                                       |
+| `--no-config-file`, `-n` / -                                    | Do not use a config file.                                                    | `false`                                      |
+
 
 ### Tags variables
 The following variables can be used in the template folders/files and/or in the `exclude_tags` list:
 * `album`
 * `album_artist`
 * `album_id`
 * `album_sort`
@@ -155,18 +157,19 @@
 * `aac-he-legacy`
 * `aac`
 * `aac-he`
 * `aac-binaural`
 * `aac-downmix`
 * `aac-he-binaural`
 * `aac-he-downmix`
-* `alac`
 * `atmos`
+* `ac3`
+* `alac`
 * `ask`
-    * When using this option, the script will ask you which **non-legacy** codec to use.
+    * When using this option, the script will ask you which **non-legacy** codec to use that is available for the song.
 
 **Support for non-legacy codecs are not guaranteed, as most of the songs cannot be downloaded when using non-legacy codecs.**
 
 ### Music videos codecs
 The following codecs are available:
 * `h264-best` (with AAC 256kbps, up to 1080p)
 * `h265-best` (With AAC 256kpbs, up to 2160p)
```

