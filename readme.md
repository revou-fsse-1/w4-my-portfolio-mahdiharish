# WEBSITE DEPLOYMENT & CUSTOM DOMAIN USING PERSONAL WEBSITE

### Hello!

This readme file will be used to document whole process of deploying website using Netlify, creating a custom domain for our personal website, and connecting it through Cloudflare to add layer of protection for our website. For my custom domain, I will be using one from Niagahoster.

For this project, I will be using my own personal website that has been created for Week 1 project.

[Personal Website](https://mahdiharish.netlify.app/)

This is my personal website with URL using Netlify.

[Personal Website with Custom Domain]()

This is my personal website with custom domain URL.

![My website's homepage](./assets/ss-home.jpg)

## HOW TO DEPLOY WEBSITE USING NETLIFY

1. Sign up/log in with Netlify. I am using my email for this, and then connect my Github repository later.

![Login/Signup to Netlify](./assets/step-1.jpg)

2. After logging in, you will be directed to team overview's page where you can review your work within Netlify.

![Team overview](./assets/step-2.jpg)

To deploy our website, we will need to click

> Add new site

which is highlighted in picture below.

![Add new site](./assets/step-3.jpg)

There will be few options available, but for now we will deploy it by importing existing projects that we have already done in our GitHub repository.

3. Based from Netlify, there are 3 steps available for this, which can be reviewed below.

![How to deploy website using Netlify](./assets/step-4.jpg)

For this, we can choose GitHub account since we are using GitHub for our repository. You need to authorize your account to GitHub so you can use it.

After that, we can choose which account and repository that will be deployed. You can search the repository by using parts of repository name. It is pretty easy.

![Choose GitHub account and repository](./assets/step-5.jpg)

Now, we can set up our website before we deploy it. There isn't much to do for now beside setting our branch into main for display.

![Set up before deployment](./assets/step-6.jpg)

You will be redirected to your website overview page, where you can review many things, including changing your website's name. However, this step is optional for now as we will be using custom domain. What previewed here is my past work before, so I have changed the website's name before. Initially the website name will be generated randomly.

![Website overview](./assets/step-7.jpg)

## SETTING UP CUSTOM DOMAIN

1. For this step, we need to purchase our own custom domain name. I am using Niagahoster for this reason for few reasons:

- Cheap and affordable,
- Plenty of options available,
- Reputable for its service since it's been around for quite long time in Indonesia.

![Niagahoster homepage](./assets/step-8.jpg)

2. You need to sign up/log in with Google Account for using Niagahoster service. It is pretty simple and straightforward step.

3. Later, we can choose which service we need. Choose **Domain** by clicking **Order Sekarang**

![Choose Domain service](./assets/step-9.jpg)

4. Next, we can pick what domain name we like. Choose what's available and its prices to our preference. You can also check if the domain's name is still available or not.

![Checking domain name's availability](./assets/step-10.jpg)

Afterwards, choose what we want and proceed to purchase it.

![Choosing domain name](./assets/step-11.jpg)

5. Complete purchase in this page.

![Purchase page](./assets/step-12.jpg)

6. After we complete our purchase and review it, we can proceed to our domain page in Niagahoster's website, which looks like this.

![Domain page in Niagahoster](./assets/step-13.jpg)

Now, we can proceed to Cloudflare to add layer of security protection for our website.

## SETTING UP CLOUDFLARE

1. Go to Cloudflare website and sign up/log in our account to start working.

![Cloudflare homepage](./assets/step-14.jpg)

2. After logging in, we will be redirected to our account's dashboard.

![Cloudflare's account dashboard](./assets/step-15.jpg)

3. Add our previously purchased domain's name at **Add site** above, and then enter our domain's name

![Add site](./assets/step-16.jpg)

4. Select plan for the website. Choose free one and click **Continue**.

![Payment plan](./assets/step-17.jpg)

5. After completing our selection, you need to complete your name server setup. Just skip steps after choosing plans and then go to **Overview** page for more details.

![Overview page](./assets/step-18.jpg)

Copy Cloudflare's nameservers and paste it to Niagahoster's overview domain page.

![Cloudflare's nameservers](./assets/step-19.jpg)

And then replace Niagahoster's nameservers with Cloudflare ones.

![Niagahoster's nameservers](./assets/step-20.jpg)

Please note that updating nameservers can take time up to 24 hours, so we need to wait for now. We can still proceed to next steps.

6. Now, we need to set up our DNS Record. Go to DNS tab on the left, and then choose DNS Management section. Click **Add Record**, and then choose CNAME for the type, and make the **Name** section _@_ and _www_, and then fill the **Target** section with our Netlify page.

![Cloudflare DNS Management](./assets/step-21.jpg)

Afterwards, we can proceed to our Netlify page to set up our custom domain page.

## SETTING UP CUSTOM DOMAIN IN NETLIFY

1. Go to our website page in Netlify, and then click **Set up a custom domain**.

![Website page in Netlify](./assets/step-22.jpg)

2. Fill our custom domain purchased before, and then click **Verify**. Afterwards, click **Add domain**.

![Add domain](./assets/step-23.jpg)

3. You can check the custom domain's settings here. Afterwards your website with custom domain should be able to go live now.

![Custom domain page in Netlify](./assets/step-24.jpg)
