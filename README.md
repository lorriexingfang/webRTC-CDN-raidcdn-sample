# RAID CDN Video Site Demo ---- Lower The Cost of Your Video Delievery

by [@RAID CDN Developper](http://demo-cloud.apps.58dahuo.com), 

<table width="100%">
    <tr>
        <td width="100"><a href="http://demo-cloud.apps.58dahuo.com"><img src="http://zifacdn.oss-cn-hangzhou.aliyuncs.com/raidcdn-logo.png" width="97px" height="71px" alt="RaidCDN logo"/></a></td>
        <td>For more information about how to implement RAID CDN on your video site, please email our customer service: xfang@actiontec.com</td>
    </tr>
</table>

## 0. Index

1. [Description](#1-description)
2. [Demos](#2-demos)
3. [Implementation](#3-implementation)
4. [License](#4-license)

## 1. Description

RAID CDN uses web browser based P2P technology to break free from traditional CDN infrastructures.
Drop one line of JavaScript on your video page, you are able lower the cost of your video delievery.
No matter what kind of video, origin or CDN(s) you use - RAIDCDN can provide answers.

To provide an easy and straightforward way for how does RAIDCDN save bandwidth, we create this sample project to illustrate that. 

RAIDCDN also offers a commercial CDN service, specifically designed for video delivery. For more information about how to implement RAID CDN on your site, please get in touch with us.

## 2. Demos
The first open browser fetches data from its original source.

![Demo ScreenShot](http://zifacdn.oss-cn-hangzhou.aliyuncs.com/sample_snapshot_1_1.png)

The second open browser fetches part of data from the first open tab.

![Demo ScreenShot](http://zifacdn.oss-cn-hangzhou.aliyuncs.com/sample_snapshot_1_2.png)

The third open browser fetches part of data from both first and secound open tabs.

![Demo ScreenShot](http://zifacdn.oss-cn-hangzhou.aliyuncs.com/sample_snapshot_1_3.png)

The fourth open browser.

![Demo ScreenShot](http://zifacdn.oss-cn-hangzhou.aliyuncs.com/sample_snapshot_1_4.png)

## 3. Implementation

1\. [**Sign up**] (http://accountsmgr.raidcdn.com/) to RAID CDN. 

Get instant access to your RAID CDN token. You will use it in 4.

2\. Install Node.js [**From Node.js**] (https://nodejs.org/)

For Ubuntu/Debian user:


```
$ curl -sL https://deb.nodesource.com/setup_4.x | sudo -E bash -
$ sudo apt-get install -y nodejs
```

3\. Install http-server

```
$ sudo npm install -g http-server
```
4\. Clone this sample code, unzip it to any place, and modify the token by editting index.html:

```
<script>token = 'TOKEN VALUE'; trafficDisplay = true; </script>
```
replace 'TOKEN VALUE' with the token you registered on 1.

5\. Enter the unzipped sample folder, and run your local video server:

```
$ cd raidcdn-sample
$ http-server
```

Done! Now the set up work is finished.

6\. To experience it, please open your local browser and visit:

```
http://localhost:8080
```

You can play the video on your local video serer.

Then if you open a new tab on your browser, you will see the current video you are watching fetches video chunk from the previous open one. And if you open more tabs, you will find there are multiple nodes (current opened browser) which provide video chunks to the one your are viewing.

7\. To view how much data RAID CDN helps you saved, please log in to http://accountsmgr.raidcdn.com/, click "Total" on left column and you will see:

![Demo ScreenShot](http://zifacdn.oss-cn-hangzhou.aliyuncs.com/total_usage.png)

which will illustrate your saving.

## 4. License

**_This sample is completely free for both non-commercial and commercial use._**
