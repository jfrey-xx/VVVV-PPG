# Video Feed HR Detection -- VVVV prototype

Using kinect2 (or webcam) + face tracking + clever (?) algo for heart-rate detection (aka PPG).

Proof of concept, do not expect it to work.

## Howto

Because current kinect2 implementation only works with 64bit version whereas face tracking relies on the 32bit, you'll have to work with 2 instances of vvvv -- i.e., add "/allowmultiple" parameter to the desktop shortcut.

* launch WriteKinect64 with vvvv 64bit
* launch TestDetectBPM_All with vvvv 32bit

## Dependencies

* vvvv, obviously: http://vvvv.org/ (tested with 45beta33.7)
* dx11 pack: http://vvvv.org/contribution/directx11-nodes-alpha (tested vvvv-packs-dx11-b33x-x86.zip - 09.10.14 [16:31 UTC] and vvvv-packs-dx11-b33x-x64.zip - 09.10.14 [16:17 UTC])
* image pack: http://vvvv.org/contribution/vvvv.packs.image (tested vvvv.packs_.image_b33-x86.zip - 02.09.14 [21:27 UTC])
* kinect2 nodes: http://vvvv.org/contribution/kinect2-nodes (tested VVVV.Nodes_.K2.zip - 28.07.14 [19:42 UTC]) 
* FFT value: https://github.com/jens-a-e/VVVV-FFT-Value (tested 123bce9d10d47ba22c041c132bb632fb60b282ae)

## Screenshot

Because it's *so* readable to add comments on top of a visual programming language:

![Commented screenshot](../doc/kinect-ppg-screenshot.png)
