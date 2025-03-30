---
title: Deploying a website
date: 2025-03-22
tags:
   - website
   - finance
---

From the outset of our plans to build a website, we aimed to minimize website operating costs to see how far we could push the idea of intentionally reducing operation costs. We did this to ensure the budget could be maximally allocated for direct support of orphans and neglected children. 

Our strategy was to use Hugo, an open-source static site generator to create a website in HTML and Markdown. It’s elegantly sufficient and responsive for simple websites like ours where the main purpose is to report our findings. Coupled with Netlify, a free website hosting service, this enabled a zero-cost solution to building and hosting websites. 

There’s only one major caveat: you need some programming experience, or at least the courage and willingness to code and persist through challenges. It’s definitely doable! There are plenty of tutorials out there (we recommend one below). And with the support of near-untapped intelligence at your disposal (think ChatGPT and GitHub Copilot), you essentially possess a programming co-pilot that allows you to use natural language to interface with code. In fact, we barely have any coding experience and got the website functioning despite running into problems (listed below). There are of course no-code solutions for generating website (like Squarespace and WordPress etc.) but this requires monthly subscription fees – which was an option we intentionally eliminated. 

In this post, we layout the general protocol for building a website via a Hugo and Netlify framework. 

**Prerequisites**

- Hugo tutorial by Envato Tuts+ 
- Unix (basic commands for interfacing with the command line)
- Visual Studio Code (for managing configurations and writing content) 

**High Level Overview**

1. Install Hugo on your computer
2. Create the Hugo website directory and files
3. Select and install a Hugo-based theme into this directory
4. Run the website for local development
5. Create a GitHub repository for your website documentation (via Visual Studio Code)
6. Connect GitHub repository to Netlify to deploy the website
7. Purchase domain address (e.g. Dynadot)
8. Assign domain address to the Netlify hosted website
9. Maintain website by pushing updates to the GitHub repository with changes automatically redeployed by Netlify 

**Troubleshooting**

<table border="1"> 
  <tr> 
    <td>‘Page Not Found’ after running <code>hugo server</code></td> 
    <td>For the Hugo-Winston theme, we found that the installation instructions did not result in a functioning website. This error was due to the lack of configuration details in the <code>hugo.toml</code> file. We corrected this by running the terminal command <code>mv config.toml hugo.toml</code></td> 
  </tr> 
  <tr> 
    <td>Non-functional Dynadot DNS settings</td> 
    <td> 
      We selected the ‘Name Servers’ option and inputted the following DNS details:<pre>dns1.p04.nsone.net 
dns2.p04.nsone.net 
dns3.p04.nsone.net 
dns4.p04.nsone.net</pre> 
    </td> 
  </tr> 
</table><br>

We want to thank the open-source community for enabling permissionless production of this website and for the knowledge gained through free online tutorials. Thank you to <a href="https://www.zerostatic.io/" target="_blank">Rob Austin</a> for the <a href="https://github.com/zerostaticthemes/hugo-winston-theme" target="_blank">Hugo Winston</a> theme and <a href="https://www.youtube.com/watch?v=hjD9jTi_DQ4" target="_blank"> Envato Tuts+</a> for the Hugo tutorial. To reciprocate, we’ve made our website’s code available on <a href="https://github.com/5A64/240927" target="_blank">GitHub</a> for review and if anyone wants to fork our repository. 

This whole procedure cost us AUD$12 (limited solely to the domain address purchase) and about 20 hours from initiation (training) to deployment. This is a testament that the barrier to building a website to get your work out there is incredibly low. Build, deploy and contribute something beautiful to the world! For us, it's the lessons learned from our philanthropy project. For you, it could be anything. 