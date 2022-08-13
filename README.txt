# One of the nice things about using the Jupyter notebook systems is that there is a
# rich set of contributed plugins that seek to extend this system. There is one
# such plugin, call ipy web rtc. Webrtc is a fairly new protocol
# for real time communication on the web. Yup, I'm talking about chatting.
# The widget brings this to the Jupyter notebook system.
#
# The image recorder lets us actually grab images from the camera stream. There are features
# for downloading and using the image as well. We see that the default format is a png file.
#
# If we call the download() function it will actually store the results of the camera 
# which is hooked up in image_recorder.image.
# First, lets tell the recorder to start capturing data

# Ok, the object that it stores is an ipywidgets.widgets.widget_media.Image. How do we do
# something useful with this? Well, an inspection of the object shows that there is a handy
# value field which actually holds the bytes behind the image. And we know how to display
# those.
# Lets import PIL Image
# And lets import io

# And now lets create a PIL image from the bytes
# And render it to the screen

# Great, you see a picture! Hopefully you are following along in one of the notebooks
# and have been able to try this out for yourself!
#
# What can you do with this? This is a great way to get started with a bit of computer vision.
# You already know how to identify a face in the webcam picture, or try and capture text
# from within the picture. With OpenCV there are any number of other things you can do, simply
# with a webcam, the Jupyter notebooks, and python!
