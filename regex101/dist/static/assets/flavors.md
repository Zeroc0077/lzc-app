# Selecting flavor

Picking a suitable flavor can be challenging, considering how many options there are depending on the language you are using.

Below is a simple cheat sheet to help you pick a suitable flavor for your language/tool, based on list of supported languages on regex101.

## Important information

The PCRE libraries are compiled in 16-bit mode to be compatible with your browser and Javascript.

**All flavors run natively in your browser!**

You can read more [here](https://github.com/firasdib/Regex101/wiki/FAQ#how-close-does-regex101-emulate-the-engines).

## Reference table

| Language   | RegEx101 Support | Comments                                                                   |
| ---------- | ---------------- | -------------------------------------------------------------------------- |
| JavaScript | **Full**         | Uses your browsers native implementation                                   |
| PHP        | **Full**         | Recent versions of PHP use PCRE2.                                          |
| Perl       | _Partial_        | Use the PCRE2 flavor for the greatest support                              |
| Python     | _Emulated_       | Emulated through PCRE but provides a good baseline                         |
| Ruby       | _Partial_        | Oniguruma and Onigmo are quite similar to PCRE in their feature set        |
| Java       | **Full**         | Newer versions of Java have greater support for variable width lookbehinds |
| C++        | **Full**         | Use the EcmaScript (JavaScript) flavor                                     |
| Golang     | **Full**         | Uses googles RE2 engine                                                    |
| .NET       | **Full**         | Uses .NET 7                                                                |
| Rust       | **Full**         | Uses the [Regex Crate](https://docs.rs/regex/1.10.3/regex/index.html)      |
| Scala      | **Full**         | Use the Java flavor                                                        |

_Note: This is a living document and subject to change. Feel free to suggest improvements [here](https://github.com/firasdib/Regex101/issues)._
