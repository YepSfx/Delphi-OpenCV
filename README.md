###Delphi-OpenCV
* OpenCV version - 2.4.9<br>
* Development environment - Delphi XE2-XE6<br>

Requires installed [Visual C++ redistributable for Visual Studio 2013][2]<br>

#####Contributors:
```
 Laentir Valetov (email: laex@bk.ru)
 Mikhail Grigorev (email: sleuthhound@gmail.com)
```
####How to install:
Download the archive [link][1].<br>
Unzip it to a convenient directory, thus get the following directory structure.<br>
```
<PROJECT_ROOT> - Directory, such as "C:\OpenCV\"
		<3rdParty>
		<bin>
		<component>
		<include>
		<opencv_classes>
		<samples>
```
Add the search path for the modules of the project in Delphi IDE (Tools-Options-Delphi Options-Library-Library path)
```
<PROJECT_ROOT>\source
<PROJECT_ROOT>\source\include
<PROJECT_ROOT>\source\include\calib3d
<PROJECT_ROOT>\source\include\core
<PROJECT_ROOT>\source\include\features2d
<PROJECT_ROOT>\source\include\highgui
<PROJECT_ROOT>\source\include\imgproc
<PROJECT_ROOT>\source\include\legacy
<PROJECT_ROOT>\source\include\ml
<PROJECT_ROOT>\source\include\nonfree
<PROJECT_ROOT>\source\include\objdetect
<PROJECT_ROOT>\source\include\video
<PROJECT_ROOT>\source\component
<PROJECT_ROOT>\resource\facedetectxml
```
where ```<PROJECT_ROOT>``` directory, which was unzipped project.<br>
Additionally, you can specify the path to the library header files FFMPEG
```
<PROJECT_ROOT>\source\ffmpeg
<PROJECT_ROOT>\source\ffmpeg\ctypes
<PROJECT_ROOT>\source\ffmpeg\libavcodec
<PROJECT_ROOT>\source\ffmpeg\libavfilter
<PROJECT_ROOT>\source\ffmpeg\libavformat
<PROJECT_ROOT>\source\ffmpeg\libavutil
<PROJECT_ROOT>\source\ffmpeg\libswresample
<PROJECT_ROOT>\source\ffmpeg\libswscale
```
Examples of using FFMPEG library header files are in the
```
<PROJECT_ROOT>\samples\FFMpeg
```
Open in Delphi IDE and compile:<br>
Examples of the use of certain functions and procedures 
```
<PROJECT_ROOT>\samples\LibDemo\LibDemo.groupproj
```
Examples of the use of video processing algorithms
```
<PROJECT_ROOT>\samples\MultiDemo\MultiDemo.groupproj
```
Examples of the use of video processing algorithms using VCL.Forms
```
<PROJECT_ROOT>\samples\VCLDemo\VCLDemo.groupproj
```
Examples of use of components.<br>
To install the components, open and install
```
<PROJECT_ROOT>\source\component\Delphi20\RAD Studio XE6.groupproj
```
When installing the components in your PATH variable must be available should the library "opencv_*.dll". 
Must also be installed visual C++ redistributable for Visual Studio 2013 is available on the [link][2]<br>
Examples of the use of components - open:
```
<PROJECT_ROOT>\samples\Components\cCameraCapture\cCameraCapture.dproj
<PROJECT_ROOT>\samples\Components\cMatchTemplate\cMatchTemplate.dproj

```
[1]: https://github.com/Laex/Delphi-OpenCV/archive/master.zip
[2]: http://www.microsoft.com/ru-ru/download/details.aspx?id=40784
