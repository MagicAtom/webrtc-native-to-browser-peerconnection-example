WebRTC native C++ to browser PeerConnection example
===============================================

This repository houses the code referenced by http://sourcey.com/webrtc-native-to-browser-video-streaming-example/

Check out the blog post for usage instructions. Enjoy :)

### 1 SetUp

Please go to [aisouard/libwebrtc](https://github.com/aisouard/libwebrtc.git), they have compiled libwebrtc for several platforms for several os.

**And download the version you prefer in their release.** This is a important step, please do not ignore or jump if you want to compile and run.

After download, just add the include and lib directory to server or client, or any other way you like is okay.

I only add the CMakeLists.txt for server, it's the same way in client. And in the server, after **include and lib dirctorys** are added, just do the following steps.

```sh
mkdir build
cd build
cmake ..
make
```

Actually you can find examples are all here, some file are losen.
If you use macos or linux to compile the client part, please go to linux branch for details.
https://chromium.googlesource.com/external/webrtc/+/5f93d0a140515e3b8cdd1b9a4c6f5871144e5dee/talk/