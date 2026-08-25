# Week 1 Plan


Day 1 - mentimeter, course intro, browser devtools trace exercise, URL dissection with unfurl, AI agent setup in VS code
  Out of class work - find your favorite live 404 error page
Day 2 - Broken website scavenger hunt, server access and setup

## Tuesday

- [Warm-up Menti](https://www.mentimeter.com/app/presentation/al5kkjb4j3kqxtynbc9qc896aedshvgg/edit?source=dashboard)
- Course introduction & syllabus overview
- [Textbook](https://ecampusontario.pressbooks.pub/webdev/)
- Browser DevTools trace exercise
- [Anatomy of a URL](https://ecampusontario.pressbooks.pub/webdev/chapter/anatomy-of-a-url/)
    - [RFC 3986](https://www.rfc-editor.org/info/rfc3986/#section-3) - Uniform Resource Identifier (URI)
    - URL dissection with [unfurl](https://dfir.blog/unfurl/)
- Development environment setup
    - VS Code
    - Github Desktop
    - Docker



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

