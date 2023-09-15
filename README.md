# FFmpegKit for RK

`FFmpegKit` is a collection of tools to use `FFmpeg` in `Android`,  `Linux`applications.

It includes scripts to build `FFmpeg` native libraries, a wrapper library to run `FFmpeg`/`FFprobe` commands in


### 1. Features
- Scripts to build FFmpeg native libraries
- `FFmpegKit` wrapper library to run `FFmpeg`/`FFprobe` commands in applications
- Supports native platforms: Android, Linux
- Based on FFmpeg `v4.5-dev` or later with optional system and external libraries


### 2. Android

See [Android](android/README.md) to learn more about `FFmpegKit` for `Android`.

### 3. Linux

See [Linux](linux/README.md) to learn more about `FFmpegKit` for `Linux`.

### 4. Build Scripts

Use `android.sh`,  `linux.sh` to build `FFmpegKit` for each native platform.


### 5. FFmpegKit Library

`FFmpegKit` is a wrapper library that allows you to easily run `FFmpeg`/`FFprobe` commands in applications. It
provides additional features on top of `FFmpeg` to enable platform specific resources, control how commands are
executed and how the results are handled.

`Android` library of `FFmpegKit` has a `Java` API,`Linux` library has a `C++` API , which are identical in terms of features and capabilities.

### 6. Packages

Please remember that some parts of `FFmpeg` are licensed under the `GPL` and only `GPL` licensed `ffmpeg-kit` packages
include them.

<table>
<thead>
<tr>
<th align="center"></th>
<th align="center"><sup>min</sup></th>
<th align="center"><sup>min-gpl</sup></th>
<th align="center"><sup>https</sup></th>
<th align="center"><sup>https-gpl</sup></th>
<th align="center"><sup>audio</sup></th>
<th align="center"><sup>video</sup></th>
<th align="center"><sup>full</sup></th>
<th align="center"><sup>full-gpl</sup></th>
</tr>
</thead>
<tbody>
<tr>
<td align="center"><sup>external libraries</sup></td>
<td align="center">-</td>
<td align="center"><sup>vid.stab</sup><br><sup>x264</sup><br><sup>x265</sup><br><sup>xvidcore</sup></td>
<td align="center"><sup>gmp</sup><br><sup>gnutls</sup></td>
<td align="center"><sup>gmp</sup><br><sup>gnutls</sup><br><sup>vid.stab</sup><br><sup>x264</sup><br><sup>x265</sup><br><sup>xvidcore</sup></td>
<td align="center"><sup>lame</sup><br><sup>libilbc</sup><br><sup>libvorbis</sup><br><sup>opencore-amr</sup><br><sup>opus</sup><br><sup>shine</sup><br><sup>soxr</sup><br><sup>speex</sup><br><sup>twolame</sup><br><sup>vo-amrwbenc</sup></td>
<td align="center"><sup>dav1d</sup><br><sup>fontconfig</sup><br><sup>freetype</sup><br><sup>fribidi</sup><br><sup>kvazaar</sup><br><sup>libass</sup><br><sup>libiconv</sup><br><sup>libtheora</sup><br><sup>libvpx</sup><br><sup>libwebp</sup><br><sup>snappy</sup><br><sup>zimg</sup></td>
<td align="center"><sup>dav1d</sup><br><sup>fontconfig</sup><br><sup>freetype</sup><br><sup>fribidi</sup><br><sup>gmp</sup><br><sup>gnutls</sup><br><sup>kvazaar</sup><br><sup>lame</sup><br><sup>libass</sup><br><sup>libiconv</sup><br><sup>libilbc</sup><br><sup>libtheora</sup><br><sup>libvorbis</sup><br><sup>libvpx</sup><br><sup>libwebp</sup><br><sup>libxml2</sup><br><sup>opencore-amr</sup><br><sup>opus</sup><br><sup>shine</sup><br><sup>snappy</sup><br><sup>soxr</sup><br><sup>speex</sup><br><sup>twolame</sup><br><sup>vo-amrwbenc</sup><br><sup>zimg</sup></td>
<td align="center"><sup>dav1d</sup><br><sup>fontconfig</sup><br><sup>freetype</sup><br><sup>fribidi</sup><br><sup>gmp</sup><br><sup>gnutls</sup><br><sup>kvazaar</sup><br><sup>lame</sup><br><sup>libass</sup><br><sup>libiconv</sup><br><sup>libilbc</sup><br><sup>libtheora</sup><br><sup>libvorbis</sup><br><sup>libvpx</sup><br><sup>libwebp</sup><br><sup>libxml2</sup><br><sup>opencore-amr</sup><br><sup>opus</sup><br><sup>shine</sup><br><sup>snappy</sup><br><sup>soxr</sup><br><sup>speex</sup><br><sup>twolame</sup><br><sup>vid.stab</sup><br><sup>vo-amrwbenc</sup><br><sup>x264</sup><br><sup>x265</sup><br><sup>xvidcore</sup><br><sup>zimg</sup></td>
</tr>
<tr>
<td align="center"><sup>android system libraries</sup></td>
<td align="center" colspan=8><sup>zlib</sup><br><sup>MediaCodec</sup></td>
</tr>
<tr>
<td align="center"><sup>ios system libraries</sup></td>
<td align="center" colspan=8><sup>bzip2</sup><br><sup>AudioToolbox</sup><br><sup>AVFoundation</sup><br><sup>iconv</sup><br><sup>VideoToolbox</sup><br><sup>zlib</sup></td>
</tr>
<tr>
<tr>
<td align="center"><sup>macos system libraries</sup></td>
<td align="center" colspan=8><sup>bzip2</sup><br><sup>AudioToolbox</sup><br><sup>AVFoundation</sup><br><sup>Core Image</sup><br><sup>iconv</sup><br><sup>OpenCL</sup><br><sup>OpenGL</sup><br><sup>VideoToolbox</sup><br><sup>zlib</sup></td>
</tr>
<tr>
<td align="center"><sup>tvos system libraries</sup></td>
<td align="center" colspan=8><sup>bzip2</sup><br><sup>AudioToolbox</sup><br><sup>iconv</sup><br><sup>VideoToolbox</sup><br><sup>zlib</sup></td>
</tr>
</tbody>
</table>

 - `zimg` is supported since `v4.5.1`

### 7. Versions

`FFmpegKit` binaries generated use the same major and minor version numbers as the upstream `FFmpeg` project. The
third and last number in the version string, if exists, is specific to `FFmpegKit`. It shows different releases from
the same `FFmpeg` release branch.

`dev` part in the version string indicates that `FFmpeg` source code is cloned from the `FFmpeg` `master` branch and
the exact version number of `FFmpeg` is obtained using the `git describe --tags` command.

|    Platforms     |                                 FFmpegKit Version                                 | FFmpeg Version | Release Date |
|:----------------:|:---------------------------------------------------------------------------------:|:--------------:|:------------:|
|  Android<br>Apple       |         [6.0](https://github.com/arthenica/ffmpeg-kit/releases/tag/v6.0)   |      6.0       | Aug 21, 2023 |
|  Android<br>Apple      |         [5.1](https://github.com/arthenica/ffmpeg-kit/releases/tag/v5.1)    |     5.1.2      | Sep 29, 2022 |
|  Android         |       [4.5.1](https://github.com/arthenica/ffmpeg-kit/releases/tag/v4.5.1)        |  4.5-dev-3393  | Jan 01, 2022 |
| Android<br>Apple |         [4.5](https://github.com/arthenica/ffmpeg-kit/releases/tag/v4.5)          |  4.5-dev-2008  | Sep 18, 2021 |
| Android<br>Apple |         [4.4](https://github.com/arthenica/ffmpeg-kit/releases/tag/v4.4)          |  4.4-dev-3015  | Mar 03, 2021 |

### 8. LTS Releases

`FFmpegKit` binaries are published in two release variants: `Main Release` and `LTS Release`.

- Main releases include complete functionality of the library and support the latest SDK/API features.

- LTS releases are customized to support a wider range of devices. They are built using older API/SDK versions, so some features are not available on them.

This table shows the differences between two variants.

|        | Main Release |                        LTS Release                        |
| :----: | :----: |:---------------------------------------------------------:|
| Android API Level | 24 |                            16                             |
| Android Camera Access | Yes |                             -                             |
| Android Architectures | arm-v7a-neon<br/>arm64-v8a<br/>x86<br/>x86-64 | arm-v7a<br/>arm-v7a-neon<br/>arm64-v8a<br/>x86<br/>x86-64 |

### 9. Documentation

A more detailed documentation is available under [Wiki](https://github.com/arthenica/ffmpeg-kit/wiki).

### 10. Test Applications

You can see how `FFmpegKit` is used inside an application by running test applications created under
[FFmpegKit Test](https://github.com/arthenica/ffmpeg-kit-test) project.

All applications are identical and supports command execution, video encoding, accessing https urls, encoding audio,
burning subtitles, video stabilisation, pipe operations and concurrent command execution.

### 11. See Also

- [FFmpeg API Documentation](https://ffmpeg.org/doxygen/4.0/index.html)
- [FFmpeg Wiki](https://trac.ffmpeg.org/wiki/WikiStart)
- [FFmpeg External Library Licenses](https://www.ffmpeg.org/doxygen/4.0/md_LICENSE.html)
