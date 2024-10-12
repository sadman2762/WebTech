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

# Topic 7 (lecture 4)
# XML 1.0

### What type of standards does XML belong to?
- De facto standards **(Correct Answer)**
- De jure standards 
- Voluntary consensus standards

### In which order must/should elements be declared in a DTD?
- An element e must be declared before any other elements that can contain the element e.
- The order does not matter. **(Correct Answer)**
- For readability, elements should be declared in alphabetical order.
- The root element must be declared first, all other elements can be declared in any order.

### Which one of the following statements is true for the following document?

    xml
    <?xml version="1.0"?>
    <person>Eminem</person>
    <person>Batman</person>
    <cat>Grumpy Cat</cat>


- This is not a well-formed XML document. (Correct Answer)
- The XML document is well-formed, but is invalid.
- The XML document is valid, but is not well-formed.
- The XML document is both well-formed and valid.
### Consider the element type declaration  ```<!ELEMENT e ((a | b)*, c)+>``` . Which of the following elements are valid according to the declaration?
-     <e> <c/> <c/> <c/> </e> (Correct Answer)
-     <e> <c/> <a/> <b/> </e>
-     <e> <a/> <b/> <c/> </e> (Correct Answer)
-     <e> <c/> <a/> <b/> <c/> </e>
-     <e></e>
### Which of the elements declared in a DTD can be used as the root element in XML documents?
- Any of them.(Correct Answer)
- Only top-level elements, i.e., elements that do not occur in the content model of any other elements declared in the DTD. 
- Only the element that is declared first in the DTD.
- Only elements marked as potential root elements in the DTD.
### Which one of the following statements is true for the following document?
    xml
    Copy code
    <?xml version="1.0"?>
    <the_beatles member="George" member="John" member="Paul" member="Ringo">
    </the_beatles>
- The XML document is both well-formed and valid.
- XML document is valid, but it is not well-formed.
- This is not a well-formed XML document. (Correct Answer)
- XML document is well-formed, but it is invalid.
### In XML, the elements declared as ```<!ELEMENT copyright (#PCDATA|holder)*>```or ```<!ELEMENT para (#PCDATA|bold|italic)*>``` are said to have ```Mixed``` content.
### Which of the following markup constructs are allowed in the content of the element e declared as <!ELEMENT e (#PCDATA)>?
- XML declaration
- Comment (Correct Answer)
- Character reference (Correct Answer)
- Entity reference (e.g., <) (Correct Answer)
- Document type declaration
- CDATA section (Correct Answer)
### How to declare the element e in a DTD as an empty element?
-     <!ELEMENT e>
-     <!ELEMENT e EMPTY> (Correct Answer)
-     <!ELEMENT e (#EMPTY)>
-     <!ELEMENT e (EMPTY)>
### Are the elements e and f allowed to be declared in a DTD as follows?
    xml
    Copy code
    <!ELEMENT e (f*)>
    <!ELEMENT f (e*)>
- No, because it could result in infinite recursion. 
- Yes.(Correct Answer)
- No, because f is declared after e, thus, it is not available in the content model of e.
- The answer is implementation-specific.
### Which one of the following is true for XML?
- Well-formedness and validity are mutually exclusive.
- Well-formedness implies validity.
- Well-formedness and validity are entirely unrelated.
- Validity implies well-formedness. (Correct Answer)
### Which one of the following statements is true for the following document?
    xml
    Copy code
    <?xml version="1.0"?>
    <title>The Fellowship of the Ring</title>
    <title>The Two Towers</title>
    <title>The Return of the King</title>
- The XML document is both well-formed and valid.
- This is not a well-formed XML document. (Correct Answer)
- The XML document is valid, but it is not well-formed.
- The XML document is well-formed, but it is invalid.
### Which one of the following element type declarations declares an element a that must contain exactly one x element and zero or more y elements, where the x and y elements can be specified in any order?
-     <!ELEMENT a (y,x,y)*>
-     <!ELEMENT a (y*,x+,y*)> (Correct Answer)
-     <!ELEMENT a (y*,x,y*)>
-     <!ELEMENT a (y*,x,y*)*>
### Is ```<!ELEMENT a (a*)>``` a valid XML element type declaration?
- Yes.(Correct Answer)
- No, because it could result in infinite recursion. 
- Yes, but if and only if the element a does not occur in the content model of other elements declared within the DTD.
- The answer depends on the settings of the XML parser.
### Which one of the following element type declarations declares an element e that must contain exactly one a element and exactly one b element, where the a and b elements can be specified in any order?
-     <!ELEMENT e (a|b)?>
-     <!ELEMENT e ((a,b)|(b,a))> (Correct Answer)
-     <!ELEMENT e ((a|b),(b|a))>
-     <!ELEMENT e ((a|b),(a|b))>

### Which of the following is a valid XML name?
- AC/DC
- 2Pac
- Will.I.am (correct)
- Da$h
### Which of the following is not a valid XML name?
- ab
- Iamsu!(correct)
- _ _1th_ _
- so...

### XML syntax of chracter references--
- \u221E
- U+221E
- &#221E
- &#x221E(correct)

### How to specify C&A in the text of XML?
    C@amp;A

### Consider the element type declaration:

xml
Copy code
```<!ELEMENT a ((b, c) | (d+, c)) +>```
where the elements b, c, and d are declared to be empty. Which one of the following XML fragments is invalid?

    A.  <a><b/><c/><b/></a>
    B. <a><d/><d/><c/><b/></a>
    C. <a><d/><c/><b/><c/></a>
    D. <a></a> (correct)

### Give an element type declaration that declares the element a with the following content model: it must contain exactly one e element and any number of (including 0) b elements, where the b and c elements can be provided in any order.

    <!ELEMENT a (b*, c*, e, b*, c*)>

  

     
