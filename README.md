<div align="center">
    <img src="./assets/repo-logo.jpg" width="80%" alt="repo-logo"/>
    <h1> Web Security Handbook </h1>
</div>

This repository was created with the intention of providing developers with insights, best practices, and practical examples to help you navigate the complex landscape of web security. Secure your web applications with confidence using the knowledge shared in this handbook.

# Table Of Contents

- [Cookies](#cookies)
  - [What are cookies on websites?](#what-are-cookies-on-websites)
  - [Where are cookies stored?](#where-are-cookies-stored)
  - [What are cookies used for?](#what-are-cookies-used-for)
  - [What are the different types of cookies?](#what-are-the-different-types-of-cookies)
  - [How do cookies affect the user privacy?](#how-do-cookies-affect-the-user-privacy)
  - [HTTP Cookies: Pros and Cons](#http-cookies-pros-and-cons)

# Cookies

### What are cookies on websites?

Cookes are small files that allow websites to remember information about you. An HTTP cookie, also known as a “web cookie,” “browser cookie,” or simply “cookie,” is a small piece of data that a server sends to a user’s web browser. After being received and stored on the browser, cookies are sent back to the server with each request. HTTP cookies generally contain information about the user’s activity and help maintain session state between different browsing sessions.

Keep in mind that HTTP is a stateless protocol. That means that the server treats each request as a stand-alone operation and has no memory of previous requests from the same user. Thus, it is necessary to send additional information with each request to maintain the state of a user’s session. This is exactly what cookies are about.

Specifically, the cookie mechanism starts when a website’s server returns an HTTP response with a Set-Cookie header. This header contains some data and an expiration date. When the browser receives a response involving a Set-Cookie header, it can store the cookie data in a text file or keep it in memory. Now, when the user visits a page on that website, the browser will send the cookie back to the server in the Cookie header of the request.

Cookies play a key role when it comes to providing a more personalized experience, maintaining login sessions, and tracking users. HTTP Cookies can also be used for security and authorization purposes.

### Where are cookies stored?

Web browsers store cookies in a designated file on users' devices hard drive. The Google Chrome web browser, for instance, stores all cookies in a file labeled "Cookies." Chrome users can view the cookies stored by the browser by opening developer tools, clicking the "Application" tab, and clicking on "Cookies" in the left side menu.

### What are cookies used for?

**State/Session Management**

HTTP cookies are used by websites to remember information about a user’s session. This information includes login sessions, search filters, the scroll position on a long page, and more. For example, when a user adds items to their shopping cart on an eCommerce website, this info is stored in a cookie. When the user closes the browser or visits another page, that valuable data is not lost but remains safe in the cookie saved on the disk.

**Personalization**

Cookies can be used to store user preferences, such as preferred language, font size, and selected colors. This information is critical to personalizing the user’s experience on the website, making it more enjoyable and accessible.

**Tracking Users**

Cookies allow tracking the behavior of a user on a website, such as which pages they visit, how long they stay on a page, and which links they click on. This data can be studied to improve the overall user experience, adapting the content or layout of pages accordingly. Also, cookies are useful for collecting analytics data. For example, Google Analytics collects data and reports site usage statistics through a set of cookies.

### What are the different types of cookies?

As you just learned, HTTP cookies are useful in a variety of circumstances. As a result, there are many different types of cookies. Let’s take a look at the most important ones:

- _Session cookies:_ Are temporary and stored in memory by the browser. They only exist until the user closes their web browser. They are used to remember information about the user’s current browsing session on a website.

- _Persistent cookies:_ They are stored on the user’s hard drive and persist even after the web browser is closed. They are typically used to remember user preferences and maintain login sessions over time.

- _First-party cookies:_ Are set by the website that the user is visiting and are used to remember information about the user’s session and preferences.

- _Third-party cookies:_ Are set by a different website than the one the user is visiting and are generally used for advertising or tracking purposes. Examples are cookies from Google Analytics, Facebook.

### How do cookies affect the user privacy?

As described above, cookies can be used to record browsing activity, including for advertising purposes. However, many users do not want their online behavior to be tracked. Users also lack visibility or control over what tracking services do with the data they collect.

Even when cookie-based tracking is not tied to a specific user's name or device, with some types of tracking it could still be possible to link a record of a user's browsing activity with their real identity. This information could be used in any number of ways, from unwanted advertising to the monitoring, stalking, or harassment of users. (This is not the case with all cookie usage.)

Some privacy laws, like the EU's ePrivacy Directive, address and govern the use of cookies. Under this directive, users have to provide "informed consent" — they have to be notified of how the website uses cookies and agree to this usage — before the website can use cookies. (The exception to this is cookies that are "strictly necessary" for the website to function.) The EU's General Data Protection Regulation (GDPR) considers cookie identifiers to be personal data, so its rules apply to cookie usage in the EU as well. Also, any personal data collected by cookies falls under the GDPR's jurisdiction.

Largely because of these laws, many websites now display cookie banners that allow users to review and control the cookies those websites use.

### HTTP Cookies: Pros and Cons

HTTP cookies are a versatile and powerful tool that covers various needs. However, they also come with some drawbacks to consider. It is time to dig into the main pros and cons of HTTP cookies.

**Pros**

1. Easy to implement and use: Cookies are a simple and effective way for maintaining session state over HTTP.
2. Can be stored on disk: Persistent cookies allow data from the previous browsing session to be retained, even after closing the browser.
3. Can be shared between pages and domains: The same cookie can be used by several pages of the same site and by different subdomains of the same domain.

**Cons**

1. Limited in size and number: Most browsers limit browser size to 4 KB and allow no more than 150 cookies per domain.
2. Can be deleted by users: Cookies can be deleted by users at any time directly in the browser, which can cause problems for websites that rely on them.
3. Security/Privacy risks: Cookies can contain sensitive information about the user and pose a security risk. Additionally, cookies can be used to track and collect data on a user’s behavior, which raises privacy concerns.
