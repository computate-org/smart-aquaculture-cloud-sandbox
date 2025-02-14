# Cloud sandbox powered by FIWARE

## About the open source GPL3 license and copyright for this product

Copyright (c) 2024 Computate Limited Liability Company in Utah, USA

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see <https://www.gnu.org/licenses/>.

ADDITIONAL TERMS

As stated in section 7. c) and e) of the GPL3 license, 
"you may supplement the terms of this License with terms," 
Computate has added the following additional terms to the license: 

  7 c) Prohibiting misrepresentation of the origin of that material, and
    requiring that modified versions of such material be marked in
    reasonable ways as different from the original version;

  7 e) Declining to grant rights under trademark law for use of some
    trade names, trademarks, or service marks;

Please do not redistribute this course until you have built your own platform with these tools, 
separate from the computate.org platform, and reconfigure your fork of this repo to deploy 
your own platform instead of the computate.org platform. 

QUESTIONS

For questions about this open source license, please contact our public mailing list at computate@group.computate.org

# Red Hat OpenShift Developer Sandbox

## How to start an OpenShift Developer Sandbox

Start a [free Red Hat OpenShift Developer Sandbox
here](https://developers.redhat.com/developer-sandbox).

<img src="pictures/10000201000002EC000000B797470F50FAD9B503.png" />

Click on the
<img src="pictures/100002010000002A00000016F8A31816B66F52D8.png" />
button in the top right corner.

<img src="pictures/10000201000000C20000004B778672F45D986E77.png" />

### Register for a free Red Hat account

If you do not already have a free Red Hat account, click
<img src="pictures/100002010000011D000000194F39C6CC5D1A0EA6.png" />.

Log in if you already have a free Red Hat account:

<img src="pictures/10000201000001A4000000F06DFE281142C79837.png" />

### Start your OpenShift Developer Sandbox

After you are logged into your Red Hat account, return to the page to
start a [free Red Hat OpenShift Developer Sandbox
here](https://developers.redhat.com/developer-sandbox).

Click
<img src="pictures/10000201000000DF000000245838DB81DC18462A.png" />

Then click
<img src="pictures/100002010000008A000000248AC83F9D6A153747.png" />

Before you can access your new sandbox, you will need to request an
activation code by phone. Click on the link.

Be sure to enter your country code, and phone number correctly, then
check your phone for the activation code.

<img src="pictures/1000020100000359000000CB3CE9E1A39B080DE6.png" />

Enter your activation code in the box .

After a few moments, you should be able to start your Red Hat OpenShift
Developer Sandbox. Click the button to start your sandbox for free.

<img src="pictures/100002010000027E0000008072F673BF670FECCA.png" />

If you see a message
<img src="pictures/10000201000001EA0000001EB1A61FBC1D9C353B.png" />,
then click
<img src="pictures/1000020100000048000000243F3A75341A965DC4.png" />

You can get started in the Red Hat OpenShift platform by clicking on the
button.

<img src="pictures/10000201000000740000007DED7012DEEE29A8D6.png" />

Log in by clicking on the
<img src="pictures/100002010000006C0000001DABF5B58FF6B1D253.png" />
button to log into the new sandbox with your Red Hat account.

Explore your new sandbox with a tour, or get started now.

<img src="pictures/1000020100000220000000A7B122DE8EA79F44F2.png" />


## Using the OpenShift Developer Sandbox

### Download the oc command
- Click the
<img src="pictures/10000201000000180000001946A6B15A7F8D3A9C.png" />
button in the top right of the Developer Sandbox.

- Click
<img src="pictures/100002010000010400000025591A5F602949BE11.png" />.
- Click the download link for your operating system.

<img src="pictures/1000020100000168000000AC979C70CCF932ABC5.png" />
- You'll need to extract the `oc` command and place it in your path,
for example in a `bin` directory in your `$HOME` directory.

```bash
mkdir -p ~/bin
tar xvf ~/Downloads/oc.tar -C ~/bin/
```


### Log into the OpenShift CLI in your terminal

<img src="pictures/10000201000000DA000000A925DC020844A89E01.png" />
- Click your username in the top right corner of the Developer Sandbox.
- Click
<img src="pictures/10000201000000BD00000025748AE357F93DE9CB.png" />.
- Click
<img src="pictures/10000201000000740000002333EFEF0BE6991D9D.png" />.
- Click
<img src="pictures/100002010000006A000000156B50A1A3B5B867E3.png" />.
- Copy the line to the clipboard that looks like this:

<img src="pictures/100002010000024F0000004C0CDBE88B1D849CC9.png" />
- Paste the command into your terminal to log in to the Developer Sandbox in the terminal.

<img src="pictures/10000201000003AC000000BE7CE02563432523F1.png" />

## Switch to the right project

It's important to make sure you are in the right OpenShift project in your terminal. 
All users are granted access to the `openshift-virtualization-os-images` project, but you do not want to use this project. 
Make sure you are using the project with your username ending in `-dev`. 

Run this command to see what projects are available to you, and what project you are currently in (marked by a `*`): 


```bash
oc projects
```

Run this command to switch to your project: 


```bash
oc project $(oc projects -q | grep '.*-dev$')
```

## Next...
If you have successfully ran all of the commands above, congratulations, you are ready to move on to the next notebook in the course. 

- If you have additional questions or issues, please [create an issue for the course here](https://github.com/computate-org/smart-aquaculture-cloud-sandbox/issues). 
- Otherwise, please continue to the next document [01-setup-openshift-ai-workbench.md](01-setup-openshift-ai-workbench.md). 
