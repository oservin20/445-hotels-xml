# 445-hotels-xml

# CSE 445 Assignment 4 - XML, XSD, and XML Processing

This repository contains the files and documentation for **CSE 445 Assignment 4**, which demonstrates knowledge of XML schema, XML validation, error injection, and XML-to-JSON transformation using C#.

---

## 📁 Repository Contents

| File                | Description                                                                 |
|---------------------|-----------------------------------------------------------------------------|
| `Hotels.xml`        | A valid XML document representing a list of 10 hotels.                      |
| `Hotels.xsd`        | XML Schema Definition (XSD) for validating the structure of `Hotels.xml`.   |
| `HotelsErrors.xml`  | Faulty version of the XML file containing 5 injected structural errors.     |

---

## 🌐 GitHub Pages Hosting

The XML and XSD files are publicly hosted using GitHub Pages:

- ✅ [Hotels.xml](https://oservin20.github.io/445-hotels-xml/Hotels.xml)
- ✅ [HotelsErrors.xml](https://oservin20.github.io/445-hotels-xml/HotelsErrors.xml)
- ✅ [Hotels.xsd](https://oservin20.github.io/445-hotels-xml/Hotels.xsd)

> Make sure the files are pushed to the root of the `main` branch and that GitHub Pages is enabled under repository settings.

---

## 🧪 Purpose of Each File

### ✅ `Hotels.xml`
- Represents a valid XML instance of hotel data.
- Includes 10 real or realistic hotels.
- Follows the schema defined in `Hotels.xsd`.
- Some hotels include multiple `<Phone>` entries and optional `Rating`/`NearestAirport`.

### ✅ `Hotels.xsd`
- XML Schema used to validate structure and attributes of hotel listings.
- Enforces required and optional elements as per the assignment.

### ⚠️ `HotelsErrors.xml`
- Modified version of `Hotels.xml` with **5 required errors**:
  1. Root element renamed to `<Hotel>`
  2. Missing required `Rating` attribute
  3. A `<Phone>` element omitted
  4. An `<Address>` element is missing its closing tag
  5. Duplicate `<Name>` tags within a `<Hotel>`

---

## 💡 How to Use These Files

1. Clone or fork this repo.
2. Use the URLs above to test XML validation and transformation in your C# program (`submission.cs`).
3. Implement:
   - `Verification(xmlUrl, xsdUrl)`
   - `Xml2Json(xmlUrl)`
   - A `Main()` method that tests both valid and invalid files.

---

## 📄 License

This repository is for educational purposes only and part of **CSE 445 - Distributed Software Development** at Arizona State University.
