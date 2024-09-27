# Topic 1 — World Wide Web

(1 question from this topic)

1. Associate the types of specifications with their publishers
- **WHATWG**: Living Standards
- **W3C**: Recommendations
- **IANA**: Media type registration
- **IETF**: RFC

2. Which one of the following organizations publishes standards called **Living Standards**?
- a.W3G
- b.ISO
- c.Ecma International
- d.WHATWG
- **Answer: D**

3.Which one of the following organizations publishes **RFC Documents**?
- a.IANA
- b.IETF
- c.WHATWG
- d.W3C
- **Answer:B**

4. Name four Web Standards that are currently developed by **W3C**.Different versions of same standards are not accepted.
- **HTML,CSS,XML,MathML**

# Topic 2 — Unicode

(2 questions from this topic)

1.Match Unicode character encodings with their characteristics
- UTF-32: The simplest Unicode encoding form.
- UTF-16: Maintains a balance between efficient access and economical use of storage.
- UTF-8: The most compact encoding in terms of the number of bytes used.

2.Associate the constructs for specifying a ± character (U+00B1) with the corresponding language/format
- \b1 CSS
- \u00b1 JSON
- &#xb1 XML
- &PlusMinus; HTML

3.How many bytes are used by the UTF-16 character encoding to represent Unicode code points?
- • 2 or 4 bytes
- • 1, 2, 3, or 4 bytes
- • 2 bytes
- • 16 bytes
- **Answer** 2 or 4 bytes
  
4.Associate the constructs for specifying a copyright sign with the corresponding language/format
- \a9 CSS
- \u00a9 JSON
- &#xa9 XML
- &Copy; HTML

# Topic 3 - IANA media types

(no questions asked)

# Topic 4 — Uniform Resource Identifier (URI)

(2-3 questions will be in the exam )

#### Which one(s) of the following URIs is/are equivalent with the URI `https://www.nasa.gov/`?
- [X] `https://www.nasa.gov`
- [ ] `https://nasa.gov/`
- [X] `https://www.nasa.gov:433/`
- [X] `HTTPS://www.NASA.gov/`
- [ ] `https://www.nasa.gov:80/`

#### Which URI component(s) can be used for submitting form data?
- [ ] Path
- [ ] Fragment Identifier
- [ ] Scheme
- [ ] Host
- [X] Query

#### What is the resulting URI obtained by resolving the relative reference `../a` when the URI `https://eg.com/p/q/r` is the base URI?
- [ ] `http://eg.com/p/q/a`
- [ ] `http://eg.com/p/q../a`
- [X] `http://eg.com/p/a`
- [ ] `http://eg.com/p/q/r/a`

#### What is the name for the component `/html/rfc7159` of the URI `https://tools.ietf.org/html/rfc7159#page-4`?  
Answer (single word only): `Path`

#### Which one(s) of the following is/are not a URI?
- [ ] `file://c:/Users/Batman`
- [ ] `mailto:me@eg.com`
- [X] `/index.html#nav`
- [ ] `geo:48.2010,16.3695`

#### What does URI stand for?
- [ ] Uniform Resource Indicator
- [ ] Universal Resource Identifier
- [X] Uniform Resource Identifier
- [ ] Unique Resource Identifier

#### What is percent encoding used for?
- [ ] Compressing HTTP headers in HTTP/2.
- [X] Escaping reserved characters and referring to characters that cannot be used directly in URIs.
- [ ] Referring to Unicode characters by their code points in CSS.
- [ ] Expressing lengths in percentages in CSS.

### What is the name of the URI scheme that is widely used by Web browsers to designate access to their internal resources, such as settings?

You must provide a **single word** only.

**Answer**: `about`

### How to represent the `#` character (Unicode code point U+0023) within the path component of an URI?

Select one:

- [x] `%23`
- [ ] `&#x23;`
- [ ] `\0023`
- [ ] `\#`

**Answer**: `%23`

#### `https://wordery.com/search?term=scotland#results` (special mention in lecture)

    |   \___/   |  \__________/   | \_____/  |  \___________/  | \_____/  |
    |  Scheme   |      Host       |   Path   |      Query      | Fragment |

- **Scheme**: `https`
- **Host**: `wordery.com`
- **Path**: `/search`
- **Query**: `term=scotland`
- **Fragment**: `results`

Let `http://example/a/b/c?q` be the base URI (special mention in lecture)

| Relative Reference | Target URI                  |
|--------------------|-----------------------------|
| `d`                | `http://example/a/b/d`       |
| `./d`              | `http://example/a/b/d`       |
| `/d`               | `http://example/d`           |
| `//localhost`      | `http://localhost`           |
| `?y`               | `http://example/a/b/c?y`     |
| `d?y`              | `http://example/a/b/d?y`     |

| Relative Reference | Target URI                  |
|--------------------|-----------------------------|
| `#z`               | `http://example/a/b/c?q#z`  |
| `""` (empty string)| `http://example/a/b/c?q`     |
| `.`                | `http://example/a/b/`        |
| `./`               | `http://example/a/b/`        |
| `..`               | `http://example/a/`          |
| `../d`             | `http://example/a/d`         |
| `../../d`          | `http://example/d`           |


#### URI comparison
#### Which one(s) of the following URIs is/are not equivalent with the URI `https://www.w3.org/`?
- [ ] `https://WWW.W3.ORG/`
- [ ] `https://www.w3.org:443/`
- [ ] `https://www.w3.org`
- [X] `https://www.w3.org:80/`

#### Name 4 URI schemes other than https or http:
**Answer**:urn,mailto,about,geo,tel

# TOPIC 5 Markdown

### Format Associations
- **Has several variants**: JSON
- **Has two concrete syntaxes**: XML
- **Originates from ECMAScript**: JavaScript
- **Has a modular structure**: XML
- **Can be used both for document-centric and data-centric applications**: JSON

### Inventor Achievements
- **John Gruber**: Markdown
- **Ethan Marcotte**: Responsive Web Design
- **Douglas Crockford**: JSON
- **Tim Berners-Lee**: World Wide Web

### Software Descriptions
- **Data transfer tool**: curl
- **Document conversion tool**: Pandoc
- **Set of text editor plugins**: Emmet
- **Text-based web browser**: Lynx

#### Markup languages are computer languages for annotating text.(special mention in class)


# Topic 6 HTTP Fundamentals

## Header Fields Usage

| HTTP Header Field  | Usage                  |
|--------------------|------------------------|
| Accept             | In request only         |
| Content-Length     | Both in requests and responses |
| Location           | In responses only       |
| Content-Type       | Both in requests and responses |
| Host               | In request only         |
| ETag               | In responses only       |

---

## HTTP Method for Metadata Retrieval

Which HTTP method can be used to obtain metadata about a resource without transferring any representation data?

- **HEAD**
- POST
- GET
- OPTIONS

**Answer:** HEAD

---

## HTTP Status Codes and Reason Phrases

| HTTP Status Code   | Reason Phrase          |
|--------------------|------------------------|
| 200                | OK                     |
| 403                | Forbidden              |
| 303                | See Other              |
| 500                | Internal Server Error  |
| 101                | Switching Protocols    |
| 401                | Unauthorized           |
| 301                | Moved Permanently      |
| 100                | Continue               |
| 503                | Service Unavailable    |
| 201                | Created                |

**Options:**

- 200: OK
- 403: Forbidden
- 303: See Other
- 500: Internal Server Error
- 101: Switching Protocols
- 401: Unauthorized
- 301: Moved Permanently
- 100: Continue
- 503: Service Unavailable
- 201: Created

---

## HTTP Method(s) for Submitting Form Data

Which HTTP method(s) can be used to submit form data?

- **PUT**
- **GET**
- **POST**
- OPTIONS

**Answer:** GET, POST

---

## HTTP Request/Response Exchange

Below is an HTTP request/response exchange:


  < HTTP/1.1 304 Not Modified < Date: Mon, 25 May 2020 19:18:21 GMT < Server: Apache/2.4.18 (Ubuntu) < ETag: "2cSe-56b208b5d1e19;5a23b68797Fce" < Content-Location: LICENSE-2.0.txt < Expires: Mon, 25 May 2020 
  20:18:21 GMT < Cache-Control: max-age=3600 < Vary: negotiate, accept

### What type of request is the above one?

- **Simple**
- **Conditional**
- **Idempotent**
- **Unsafe**

**Answer:** Conditional
Give a Practical use case of this kind of request:

---

## User-Agent Header Field

Each HTTP request should include a header field that contains information about the client program (e.g., information about the operating system on which the client runs) initiating the request. What is the name of this well-known header field?

- **User-Agent**
- Accept
- Content-Type
- Host

**Answer:** User-Agent

---

## Characteristics of HTTP/1.1

Which of the following are characteristics of HTTP/1.1?

- **Stateful**
- **Text-based**
- **General-purpose**
- **Stateless**
- **Binary**
- **Special-purpose**

**Answer:** Text-based, General-purpose, Stateless


What is a session?
- Session is a sequence of request and response between client and servers.

What is main difference between the response of HEAD and response of GET method?
- The response of HEAD identical to GET but its without the message body or content



