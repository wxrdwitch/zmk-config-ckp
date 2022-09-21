# bb!
You made it! I'm so proud of youu x

So, this is the place where your keyboard configuration is going to happen. Due to some (100% totally, definitely planned, for sure) pleasant surprises about how your keyboard works, you don't even really have to download anything. You can do it all here from GitHub.

Before we get started, your keyboard is the BT60, created by a smol company called PolarityWorks. Your layout wasn't too much like the default options (ANSI enter key, iso \\|, split right shift), so I went ahead and modified the relevant file, which you shouldn't have to touch... unless I fucked up...

Firmware is a variety of software that interacts directly with the hardware. In this case, it's the software that reads when one of many switches is pressed and then produces a signal that a computer can understand. The difference between your 'ZMK' firmware and that of most keyboards is that you can do a lot of clever things. As a result, I'm sure that you'll want to start messing around with things, and changing everything up, and especially eager to put Workman onto your keyboard :)

I've given you some defaults so that you have a jumping-off point. I haven't been able to test it on your actual physical keyboard in Brighton (being on a train somewhere between London Paddington and Stroud makes that pretty difficult), and I'm sure that I've got something wrong somewhere.

So you'll want to "fork this repository". A repository (or repo) is simply a collection of files, but including all the changes that have happened to those files since they were created. This means you can track how things change and revert mistakes. Forking is when you copy someone else's repository so that you can make your own changes to it without needing to ask them or breaking other people's code.

# Make an account

Pretty easy, you might even already have one, idk. Just sign up/in at the very top right.

# Fork this repo

Now you've logged in, there's a gray button that literally says "Fork", which you wanna hit after you finish reading this. You need to tick the box so that you copy across ALL the branches, not just the 'main' branch. If you miss it, don't worry, you can delete your fork and try again :)

# Get customising

You'll spend most of your time in the `bt60.keymap` file, which is where you specify most of the behaviour of your keyboard, such as what letters correspond to which presses. Click into the `config` directory and you should find it. I've put some explanation in there, but if you click the pencil icon at the top right of the text box, then you can start editing it. After you're done changing things up, just scroll down and save the changes. You can add a cute explanation here if you want to, but it's not necessary.

# Build the firmware

So, you can't just thwap that file directly onto the keyboard, you need to turn it into something that the keyboard's little onboard computer (or rather, microcontroller) understands. That's usually called compiling or building.

Click into the "Actions" tab and it should warn you that workflows aren't being run in this repo. That's Just Fine, click "I Understand", and automatic building should be enabled. Now, whenever you save a change it will try to re-compile the firmware.

Now, it will take little while. Maybe a couple minutes, but it shouldn't be super super long. It is faster to compile when you're doing things on your own computer, but we can worry about that only if we need to.

# Download it

Within the Actions tab, click on the latest build that happened in your branch ("bt60-nera"). Scroll down and there should be a box named "Artifacts" that contains a file named "firmware.zip", which contains a file named `bt60.uf2`. This is your compiled and complete firmware!

# Flash it

Your keyboard has a fantastic feature that means you don't need any special software on your computer to flash your firmware onto it. If you turn your board over and look in that little square hole, you'll see a teeny button. You might need a chopstick, but press that twice realquick with your keyboard plugged in, and it should just come up as a USB storage device (like a USB stick). Drag the `bt60.uf2` onto the device and eject it.

You might need to reset the keyboard (one way is to unplug+plug) but you should find that your new settings have been written onto the hardware, and you're up and typing!

I love you a lot, and I hope that you enjoy this procedure at least somewhat xxxx

# Troubleshooting

Come ask me about it bb, and I'll explain everything that I know ;)
