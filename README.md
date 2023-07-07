# Week 4 Assignment
## Introduction

<h1>Hello there! My name is Haibin (Uchiha)! 😁 <img src="https://media.tenor.com/6IFqFzfiC5IAAAAC/naruto-itachi.gif" width="700px" height="400px" /></h1>

This is assignment in week 4 on Full-Stack Engineering - Frontend Infra **(Deployment,Networking,Domain,Workflow).**

## Deploy Link

https://www.haikalbintang.site/

## How to clone repo until running your computer

### Make a New Empty Folder

To create a new empty folder you can use a command, or with file explorer

Command for Windows:
```
mkdir folder_name
```

### Open folder with VS Code
### Download Repositories

Download the repository onto your computer using the `git clone` command. The repository url can be seen in the desired repository.

```
git clone "<url repository>"
```

### Update Repositories

Update the repository that has been downloaded to the computer using the `git pull` command.

```
git pull origin <branch name>
```

### Uploading Changes

Before pushing, don't forget to pull first.

Add new file or change file

```
git add <file name>
```

Or you add new file or modify multiple files at once

```
git add .
```

Confirm file additions or changes

```
git commit -m "<commit messages>"
```

Submit changes to the repository

```
git push origin <branch name>
```

### Branching

Branches are used to develop new features or change source code without impacting other branches. The master branch is the default branch of a repository. Use another branch to do development and merge it back into the master branch.

#### View the branches contained in the local repository

```
git branch
```

#### Create a new branch in the local repository and send it to the remote repository

**Make new Branch**

```
git branch <new branch name>
```

**Active the new branch**

```
git checkout <new branch name>
```

**Confirm file additions or changes**

```
git commit -m "<commit messages>"
```

**Submit changes to the repository**

```
git push origin <new branch name>
```

#### Merges another branch into the active branch

**Activate the desired branch**

```
git checkout <branch name active>
```

**Update branch local**

```
git pull origin <branch name active>
```

**Merger File**

```
git merge <the name of the branch to be merged>
```

**Check and resolve conflicts due to merging branches**

```
git status
```

**Confirm and upload merging branches**

```
git commit -m "<commit messages>" -a
git push origin <branch name active>
```

#### Delete Branch

**On the remote repository**

```
git push origin :<branch name>
```

**In local repository**

```
git branch <nama branch> -d
```

## Deploy Documention 💻⚙

### Buy Domain

**Step 1 :** First you have to buy a domain at [Niagahoster](https://www.niagahoster.co.id/)

![Alt text](img/niaga_front.png)

**Step 2 :** On the domain name, it's up to you to put the domain name according to your own needs.

![niaga_domain](img/niaga_domain.png)

**Step 3 :** After choosing a domain name is done, make a payment.

![niaga_dashboard](img/niaga_dashboard.png)

Now your domain arleady done.

### Deploy Your Website in Netfliy

**Step 1 :** Open **[Netlify](https://app.netlify.com/)** and Login.

![netlify_homepage](img/netlfliy_homepage.png)

**Step 2 :** Go to tab **"Team Overiew"**

**Step 3 :** Click **"Add new Site"**

![netlify_dashboard](img/net_dashboard.jpg)

**Step 4 :** Click **"Import an existing project"**

![netlify_save](img/net_save.png)

**Step 5 :** Select your repository from Github

![netlify_repo](img/net_repo.jpg)

**Step 6 :** Pick an Owner

**Step 7 :** Pick branch main

**Step 8 :** Click **Deploy Site**

![netlify_deploy](img/net_deploy.png)

**Step 9 :** After you deploy, you will get the site name

**Step 10:** Click **Domain Settings**

![netlify_domain_setting](img/net_domain.png)

**Step 11:** Choose the site name and Edit the site name

**Step 12:** Fill the site name and Click **Save**

![netlify_changesite](img/net_changesite.png)

### Custom DNS

After you have done **Buy Domain & Set Up Netlify**, now we set up the Custom DNS.

**Step 1:** Login or create a new ID at [Cloudfare](https://www.cloudflare.com/).

**Step 2:** Enter the Domain that you bought in **Niagahoster**

![cloud_domain](img/cloud_domain-2.png)

**Step 3 :** Go To DNS Tab - Click "Add Record"

![dnsrecord_setup](img/cloud_addrecord.png)

**Step 4 :** Choose the type to **"CNAME"**

**Step 5 :** Name **www**

**Step 6 :** Copy and Paste your **Netlify** Subdomain to Target & Click **Save**

![dnsrecord_newrecord](img/cloud_dns.png)

**Step 7:** Go To **"Domain Settings"** on **Netlify**.

![net_domainset](img/net_domainset.png)

**Step 8:** Click **Add a domain**.

![net_adddomain](img/net_adddomain.png)

**Step 9::** Enter your Custom Domain Name that you bought at **Niagahoster** and Click **Verify**.

![net_setupdomain](img/net_setupdomain.png)

**Step 10 :** Done, your domain is now the main domain.

![primary_domain](iomg/../img/primary_domain.png)

### Change Your Nameservers

Don't forget change your Nameserver value

**Step 1 :** Go To **Niagahoster** and Click **Kelola Layanan**.

![niaga_dashboard](img/niaga_dashboard.png)

**Step 2 :** Go to tab Overview Domain and Click **Change Nameserver**.

![niaga_change](img/niaga_change.png)

**Step 3 :** Go to **Cloudfare** DNS Tab and see Cloudfare Nameserver and copy server values.

![cloud_value](img/cloud_value.png)

**Step 4 :** The value copied on **Cloudflare**, paste the value in Update Nameserver on **Niagahoster** and Click **Save**.

![niaga_update](img/niaga_update.png)

Done Now Your Value Nameserver arleady change.

![niaga_value](img/niaga_value.png)

### Website Launch

After we have done all the steps above, we wait for the nameserver status to be **active** on **Cloudflare**.

![cloud_active](img/cloud_active.png)

or you can get notification in email, if server arleady **active**.

![cloud_email](img/cloud_email.png)

Now you can run your website.

I hope the steps above can help you.

Thank You.

<img src="https://gifdb.com/images/high/tanjiro-demon-slayer-smile-ug5qxtabnbi4yebd.gif"  width="465px" height="262px"/>
