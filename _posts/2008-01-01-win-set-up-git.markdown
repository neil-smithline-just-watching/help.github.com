---
layout: default
title: Set Up Git
description: A quick guide to help you get started with Git
---

<p class="intro">
  If you are brand new to Git and GitHub, you&#8217;re in the right place. 
  This page will walk you through quickly getting set up with Git on Windows.
</p>

<p class="intro">This is the guide for setting up git in <strong>Windows</strong>. There are also guides for <strong><a href="/mac-set-up-git">OSX</a></strong> and <strong><a href="/linux-set-up-git">Linux</a></strong>.</p>

##<span class="step">First:</span> Download and Install GitHub for Windows

At the heart of GitHub is an open source version control system (VCS) called Git&#42;. Created by the same dudes that created Linux, 
Git is responsible for everything GitHub related that happens locally on your computer.

_&#42;If you don&rsquo;t already know what Git is, <a href="http://progit.org/book/ch1-3.html" target="_blank">take a crash course.</a>_

Git used to be unwelcoming to Windows users and required many configuration options and steps to install. 
GitHub for Windows simplifies all that into a single click to install!

<ol>
  <li>
    <p><span class="step-title">Download and install <a href="http://windows.github.com/" target="_blank">GitHub for Windows</a>.</span></p>

    <p>Click on the green _download_ button in the top right to launch the ClickOnce installer.</p>

    <img src="/images/gh4w/gh4w-click-once-install.png" width="558" height="346" alt="ClickOnce" />

    <p>We recommend clicking the _Install_ button. If you are not running as an admin, you may be prompted with 
      the User Account Control (UAC) Prompt.
    </p>

    <img src="/images/gh4w/gh4w-uac-prompt.png" width="558" height="346" alt="UAC" />
    
    <p>This will download and install GitHub for Windows.</p>

    <img src="/images/gh4w/gh4w-app.png" width="558" height="332" alt="GH4W" />

    <p>That&#8217;s it! You are done. GitHub for Windows will silently update itself when updates are available.</p>
  </li>
</ol>

##<span class="step">Advanced:</span> Set Up SSH Keys

GitHub for Windows uses HTTPS by default. Setting up SSH keys is not required, but if you prefer to use SSH, keep reading.

We use SSH keys to establish a secure connection between your computer and GitHub. Setting them up is fairly easy, but does involve a number of steps.

To make sure you generate a brand new key, you need to check if one already exists. First, you need to open Git Bash (not the Windows command line), found in the Start Menu in the "git" folder.

<img src="/images/bootcamp/bootcamp_1_win_gitbash.jpg" width="558" height="300" alt="Open the terminal" />

<div class="more-info">
  <h4 class="compressed">Need a quick lesson about Git Bash?</h4>
  <div class="more-content">
    <p>Code blocks like those on this page are part of a scripting language called Bash. To use Bash scripts, we need to use an application that was installed with Git called Git Bash.</p>

    <h4>Input</h4>
    <pre class="terminal bootcamp">
      <span class="codeline">$ echo 'This is input text'<span>This tooltip tells you what's going on.</span></span>
    </pre>

    <p>A line that begins with the dollar sign ($) indicates a line of Bash script you need to type. To enter it, type the text that follows the $, hitting the return key at the end of each line. You can hover your mouse over each line for an explanation of what the script is doing.</p>

    <h4>Output</h4>
    <pre class="terminal bootcamp">
      <span class="bash-output">This is output text.</span>
    </pre>

    <p>A line that does not begin with a $ is output text that is intended to give you information or tell you what to do next. We&rsquo;ve colored output text green in these bootcamp tutorials.</p>

    <h4>User Specific Input</h4>
    <pre class="terminal bootcamp">
      <span class="codeline">$ echo '<em>username</em>'<span>Outputs the text in the quotation marks.</span></span>
    </pre>

    <p>Areas of yellow text represent your own personal info, repos, etc. If it is part of an input ($) line, you should replace it with your own info when you type it. If it is part of output text, it is just for your reference. It will automatically show your own info in Git Bash.</p>

    <p><strong>Good to know</strong>: There will be times when you type code, hit return, and all you are given is another prompt. Some actions that you execute in Git Bash don&rsquo;t have any output. Don&rsquo;t worry, if there is ever a problem with your code, Git Bash will let you know.</p>

    <p><strong>Good to know</strong>: For security reasons, Git Bash will not display what you type when entering passwords. Just type your password and hit the return key.</p>
  </div>
</div>

{% include ssh_setup.markdown %}

##<span class="step">Then: </span> Set Up Your Info

When you first run GitHub for Windows, it will walk you through cofiguring your personal information. 
But if you prefer to use the command line.

{% include email_setup.markdown %}

##<span class="step">Lastly:</span> Celebrate

Congratulations, you now have Git and GitHub all set up! What do you want to do next?

<ol class="next-steps">
<li>Set Up Git</li>
<li><a href="/create-a-repo/">Create A Repository</a></li>
<li><a href="/fork-a-repo/">Fork A Repository</a></li>
<li><a href="/be-social/">Be Social</a></li>
</ol>
<script>
  $('#os').html("<b>" + $.client.os + "</b>");
</script>
