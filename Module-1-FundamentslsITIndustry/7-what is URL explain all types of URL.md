# What Is a URL?

A **URL (Uniform Resource Locator)** is the address used to identify and locate a resource on a network, most commonly a webpage or file on the web. A browser uses a URL to know where to send a request and which resource to ask for.

For example:

`https://www.example.com:443/products/item?id=25#details`

## Parts of a URL

A URL may contain several parts:

- **Scheme or protocol (`https`):** Indicates how the resource is accessed. Common web schemes are `http` and `https`.
- **Host or domain (`www.example.com`):** Identifies the server. A domain name is resolved to a network address.
- **Port (`443`):** Optionally specifies a network port. Standard ports are often omitted from visible URLs.
- **Path (`/products/item`):** Identifies a resource or route on the host.
- **Query string (`?id=25`):** Optional parameters sent with the request. It starts with `?`, and multiple parameters are often separated by `&`.
- **Fragment (`#details`):** Points to a section or location within a resource. The fragment is generally handled by the browser and is not sent to the server as part of the HTTP request.

Not every URL contains every part. A short URL such as `https://example.com` has no visible path, query, or fragment.

## Common Types and Forms of URLs

URLs can be classified in different ways, so these categories are not all mutually exclusive.

### 1. Absolute URL

An absolute URL gives the complete address, including the scheme and host.

Example: `https://www.example.com/images/logo.png`

It can be used from a different website or document because it identifies the host explicitly.

### 2. Relative URL

A relative URL gives a path or resource location relative to the current page or a site's base address. It does not include a scheme and host.

Examples:
- `images/logo.png`
- `/contact`
- `../products`

Relative URLs are commonly used for links and resources within the same website.

### 3. HTTP and HTTPS URLs

- **HTTP URL:** Uses the Hypertext Transfer Protocol, for example `http://example.com`.
- **HTTPS URL:** Uses HTTP protected by TLS encryption, for example `https://example.com`.

HTTPS helps protect data in transit and authenticate the website connection. It does not by itself guarantee that a site is trustworthy or that its content is safe.

### 4. `www` and Non-`www` URLs

Examples:
- `https://www.example.com`
- `https://example.com`

These are different hostnames. A website administrator may configure them to serve the same site or redirect one to the other; they are not automatically identical.

### 5. Static and Dynamic URLs

- **Static-looking URL:** Often points to a fixed page or file, such as `https://example.com/about`.
- **Dynamic URL:** Often includes query parameters used to select or change content, such as `https://example.com/search?q=books&page=2`.

This distinction describes how an application uses an address; a URL's appearance alone does not reliably reveal how the server generates its content.

### 6. Special-Purpose URLs

Some URLs use schemes for purposes other than ordinary web pages:

- **`mailto:`** Opens or creates an email message, such as `mailto:help@example.com`.
- **`tel:`** Represents a telephone link, such as `tel:+15551234567`; support depends on the device and application.
- **`ftp:`** Historically used to access files with File Transfer Protocol; support varies, and it is not the same as secure web browsing.
- **`file:`** Refers to a local file, such as `file:///...`; it does not identify a normal public website.

Only use links and schemes from sources you trust, particularly when they open files or launch another application.

## URL vs. Domain Name

A **domain name** is the human-readable name of a host, such as `example.com`. A **URL** can include that domain plus a scheme, path, query, fragment, and other optional parts.

For example, in `https://example.com/courses?level=beginner`, `example.com` is the domain name and the entire string is the URL.

## URL vs. URI

A **URI (Uniform Resource Identifier)** is a general identifier for a resource. A **URL** is a kind of URI that specifies how or where to access a resource. In everyday web use, people commonly say “URL” to mean a web address.

## Safe Use of URLs

- Check the domain spelling before entering passwords or payment details.
- Prefer HTTPS, but remember that HTTPS alone does not prove a site is legitimate.
- Be cautious with shortened links because their final destination may not be visible.
- Avoid sharing URLs that contain private tokens or sensitive information in query parameters.

## Conclusion

A URL is an address that identifies where a network resource can be accessed. It can include a scheme, host, path, query, and fragment. URLs may be absolute or relative, use HTTP or HTTPS, include static-looking paths or dynamic parameters, or use special-purpose schemes. Understanding URL parts helps people navigate websites and recognize potentially unsafe links.