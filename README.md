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









