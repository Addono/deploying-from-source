# Deploying From Source

## Modern web-app

For this exercise, we will be deploying a semi-static web-app directly from our source-control in GitHub to various providers. 
The application we will be deploying is an alternative UI for Hacker News.

We will be deploying to the following providers:
 - Vercel
 - Netlify
 - AWS Amplify

1. Fork [this repo](https://github.com/Addono/nextjs-hackernews) from GitHub into your personal organisation
2. Setup deployment from GitHub
    * Vercel
        1. Login or register at https://vercel.com 
        2. “Add new …” > “Project” > “Import from Git” > Select forked repo from GitHub
    * Netlify
        1. Login or register at https://app.netlify.com/ 
        2. “Add new site” > “Import an existing project” > “GitHub” > Select forked repo
    * AWS Amplify
        1. Login to AWS Console, details can be found at https://intra.eficode.com/display/ITSEC/Accessing+Eficode%27s+test+AWS+accounts 
        2. Navigate to AWS Amplify page (easiest to use the search bar at the top)
        3. “Get Started” > “Host a web-app” > “GitHub” > Select forked repo > Click “Next” on all defaults > “Safe and deploy”
        4. (After you’re done) Delete the Amplify App
3. (Optional) Configure custom domain

Let's see what we have:
- Open up `/api/hello`
- Make commit, observe rebuild
- Performance comparison
    - Local lighthouse
    - Observe latency characteristics https://tools.bunny.net/http-test
        - Cache misses
        - Deployment region
        - Compare to:
            - https://news.ycombinator.com
            - https://hacker-news.firebaseio.com 
- PRs, preview URLs and promoting old releases


<!--

Deploy Realworld Redwood app

1. Fork repo from GitHub

-->
