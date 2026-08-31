# Week 1 Plan

<!-- 
Day 1 - mentimeter, course intro, browser devtools trace exercise, URL dissection with unfurl, AI agent setup in VS code
  Out of class work - find your favorite live 404 error page
Day 2 - Server access and setup, start writing TaskHelm
-->

## Tuesday

- [Warm-up Menti](https://www.mentimeter.com/app/presentation/al5kkjb4j3kqxtynbc9qc896aedshvgg/edit?source=dashboard)
- Course introduction & syllabus overview
- [Textbook](https://ecampusontario.pressbooks.pub/webdev/)
- Browser DevTools trace exercise
- [Anatomy of a URL](https://ecampusontario.pressbooks.pub/webdev/chapter/anatomy-of-a-url/)
    - [RFC 3986](https://www.rfc-editor.org/info/rfc3986/#section-3) - Uniform Resource Identifier (URI)
    - URL dissection with [unfurl](https://dfir.blog/unfurl/)
- Development environment setup
    - [**VS Code**](https://code.visualstudio.com/)<br>
        Also install these extensions:
        - **Dev Containers** extension
        - **Live Preview** extension
        - **Remote - SSH** extension
    - [**Github Desktop**](https://desktop.github.com/download/)
    - [**Docker Desktop**](https://www.docker.com/products/docker-desktop/)


## URL Fun

### Deconstruct:

1. `https://example.com`
2. `https://berry.edu/academics/computer-science`
3. `http://localhost:8000/index.html#overview`
4. `https://example.com/search?q=web+dev&week=1`
5. `https://test-example.com/course/csc245/lab?section=2&mode=checkoff#rubric`
5. `http://92.168.77.18:8000/feed/245/lab?section=2&mode=checkoff#rubric`


### Domain Inference Challenge
In this section, the primary domain is hidden as `[domain]`. Your job is to infer what type of site it likely is and propose one plausible domain.

For each URL:
- Identify clues from subdomain, path, query string, and fragment.
- Infer likely site category (news, docs, e-commerce, university, etc.).
- Propose one plausible primary domain.

1. `https://support.[domain]/kb/article/4281/reset-password?source=chatbot#step-3`
2. `https://api.[domain]/v1/courses/csc245/assignments?week=1&format=json`
3. `https://store.[domain]/products/mechanical-keyboard?color=black&layout=tenkeyless#specs`
4. `https://admissions.[domain]/apply/first-year?term=fall-2026#requirements`
5. `https://docs.[domain]/guides/deploy/static-site?env=prod&region=us-east#troubleshooting`


### Build a Plausible URL from Prose
For each description, write one plausible URL that matches the task. Your URL should use sensible path structure and, when appropriate, a query string or fragment.

1. An Instagram-style social media post page that opens directly to the comments section for a specific post.
2. An Amazon product search page for noise-canceling headphones filtered to under $200 and sorted by rating.
3. A Slack-like B2B app page that opens a specific team's channel and jumps to a pinned message.
4. A GitHub issue tracker page that searches for bugs labeled "high priority" and shows only open items.
5. A Shopify admin dashboard page that opens directly to the shipping settings for one online store.


### Practice Identifying Deceptive URLs

(From https://courses.lumenlearning.com/suny-informationliteracy/chapter/understanding-urls/)

The immediate benefit of the drill below will be to improve your ability to distinguish between real and fraudulent sites, but the exercise will also help you sharpen your overall URL-analysis skills by heightening your attention to the component parts of URLs.

A) Which of the following are eBay.com web pages? Do not go to the sites. (Some sites masquerading as legitimate sites may contain harmful underlying code). Just examine the URLs.

- `http://pages.ebay.com`
- `http://movies.half.ebay.com`
- `http://pages.ebey.com`
- `http://68.112.112.34:8866/ebay.htm`
- `http://signin.ebay.com@10.19.29.2`
- `http://pages.@ebay.com`
- `http://signin-ebay.com`
- `http://www.ebay.com/electronics/ipad`
- `http://www.ebay.deals.com`
- `http://www.ebay.pro`
- `http://www.ebay.com.bb/motors/motorcycles`
- `http://www.ebay.com/itm/A-Planet-of-Viruses-by-Carl-Zimmer-2011-Hardcover-/191063912359`

B) Find the domain name in this URL:

`http://www.bankofamerica.com.sas.signon.do.detect.2.signin.sessionid.rmrlfbqjlokcjpczgs.oxcvsvcpdsoeeseytje.yucfnjtidbvnujxrwjmsea.zydyilpnchtjrriiszti.zydyilpnchtjrriiszti.zydyilpnchtjrriiszti.zydyilpnchtjrriiszti.nuyovbuskl.bernadinec.com/index.php?pageType=708XeMWZamp;cust=redacted@redacted.redactedamp;l=lWXS3AlBXVShqAhQRfhgTDrf=nttps://sitekey.bnkofamerica.com/sas/signon.do?SignIn&SMSESSIONID=ASERTFGUY2I94O0389GYBH23JNMKUYH83JMN12I90U82HJNASDKOASD9AS8D&iv=90832yhIopOWjos`


## Docker setup prompt

> Create a devcontainer setup using Docker compose for a standard LAMP server with an Apache/PHP web service and a  MySQL database service. 
> - The web service should have common ubuntu utilities installed like curl, iputils, ping, less, emacs, sudo, git, sqlite. 
> - Mount project source into the web container. 
> - Expose web and db ports for local development. 
> - Configure `devcontainer.json` to use the web service and include useful PHP/MySQL VS Code extensions
> 


## Development Work

- Get Github repos
- Access csproj server via SSH
- Start the ToDo App!





## Assignment: Extensions and Explorations

If you are not sure how to go about any of these, please ask!

> **Pick any 3, at least, of the following to work on**. Create an `assignments/homework01` directory in your repo and submit your work there in the form of text or markdown files, screenshots, or other appropriate formats. 

1. **HTTP Observation Journal**: Capture a set of interesting browser requests triggered by a single URL access to a site of your choice; Record anything interesting you see about method, status code, or resource types. What status codes do you observe for various resources and what do they mean?

2. **404 Page Field Find**: Find a live interesting and creative 404 page, capture the URL that triggered the 404 response, and describe how the path likely produced a not found response. Take a screenshot of the Network tab in DevTools showing the 404 response and include it in your submission.

3. **URL Intent Spotter Log**: During normal browsing over the week, record three interesting URLs and classify each by intent (for example: search, account/profile, filtered content, docs, checkout). For each URL, label scheme, host, path, query string, and fragment (if present), then explain which path segments or query parameters reveal that intent.

4. **JSON API URL Exploration**: Find one URL that returns JSON from a public JavaScript API. Document the base URL and test at least three variants by changing query parameters or path values. For each variant, record the exact URL, what parameter or path change you made, and how the returned data changed.

5. **Server Build-from-URL Challenge**: Given a public URL on the departmental server, create the folder and file structure needed so the URL resolves correctly. Submit the final path you created plus a quick verification note.



## Reading

Read the following chapters from the textbook: **1, 2, 4, and 5**

There are no coding practice assignments associated with the reading, but you should complete the "Check Your Understanding" questions on your own.
