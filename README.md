# splitmuxsink-multifilesink

g_object_set(G_OBJECT
(data.splitmuxsink),"location","video%%05d.mp4","max-files",4, NULL);

This is not working...there is no file named video001. It making serveral
files named 00001,0002 and after re-run it overrides same file. Plz help
me. It is my 10th day on same problem.
And how can i change the location to another folder do u people have
something for that because when i used multifilesink there is a "location"
in that i put my location like /home/shubham/spl/Videos/video.mp4  it makes
video of video.mp4 but then it do not split after writing this(below code)
it overrides same file because of same name it found(video.mp4)...plz help
me in detail or i will die solving these problems

        g_object_set(G_OBJECT
(data.multifilesink),"location",""/home/shubham/splintng/Videos/video.mp4",0,
NULL);
        g_object_set(G_OBJECT (data.multifilesink),"next-file",
4,"multifilesink", 0, NULL);
        g_object_set(G_OBJECT (data.multifilesink),
"index",rand(),"multifilesink", 0, NULL);
g_object_set(G_OBJECT (data.multifilesink), "max-file-size", 1000000,
"multifilesink", 0, NULL);
        g_object_set(G_OBJECT (data.multifilesink), "max-files", 5,
"multifilesink", 0, NULL);
