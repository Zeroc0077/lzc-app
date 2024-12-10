# 12.0.11 - 1st of November, 2024

1. Add support for new quantifier shorthand in PCRE2 10.43 [https://github.com/firasdib/Regex101/issues/2370](https://github.com/firasdib/Regex101/issues/2370)

2. Fix issue where network errors could cause uncaught exceptions in rare occasions

# 12.0.10 - 13th of October, 2024

1. Fix delete code saving, again

# 12.0.9 - 13th of October, 2024

1. Hotfix for broken dependency

# 12.0.8 - 11th of October, 2024

1. Fix issue where delete codes were not actually being stored on the client

# 12.0.7 - 1st of October, 2024

1. Fix major performance regression when handling large amount of matches

# 12.0.6 - 29th of September, 2024

1. Ensure preview generation remains functional in longer runner sessions

# 12.0.5 - 26th of September, 2024

1. Fix unit tests validation not working as intended [https://github.com/firasdib/Regex101/issues/2355](https://github.com/firasdib/Regex101/issues/2355)

2. Fix intermittent crashing of preview renderer

3. Fix crash casued by very large lines with whitespace

# 12.0.4 - 23rd of September, 2024

1. Fix issue where some users could not load the website when signed in

# 12.0.3 - 22nd of September, 2024

1. Fix theme initialization issue [https://github.com/firasdib/Regex101/issues/2351](https://github.com/firasdib/Regex101/issues/2351)

2. Make benchmark duration configurable [https://github.com/firasdib/Regex101/issues/2350](https://github.com/firasdib/Regex101/issues/2350)

# 12.0.2 - 21st of September, 2024

1. Fix saving and loading of settings

# 12.0.1 - 21st of September, 2024

1. Remove Stripe donation link

# 12.0.0 - 21st of September, 2024

This is a major rewrite of the application, where the entire application has more or less been
updated, refactored and improved from the ground up. This was done in order to stay in line with
industry leading best practices, and reduce technical debt.

While this is likely to have introduced some new quirks, it has undoubtedly fixed many.

The list below highlights some of the minor improvements you can expect:

1. Smaller bundle size (less data over the wire)

2. Improved performance and stability

3. Add new account category for all types of related entries, fixes [https://github.com/firasdib/Regex101/issues/2310](https://github.com/firasdib/Regex101/issues/2310)

4. Fix login intermittently not working, fixes [https://github.com/firasdib/Regex101/issues/2307](https://github.com/firasdib/Regex101/issues/2307)

5. Add comments addressing JS code sample [https://github.com/firasdib/Regex101/issues/2300](https://github.com/firasdib/Regex101/issues/2300)

6. Upgrade golang to support latest features [https://github.com/firasdib/Regex101/issues/2311](https://github.com/firasdib/Regex101/issues/2311)r

7. Fix golang substitution edge case [https://github.com/firasdib/Regex101/issues/2289](https://github.com/firasdib/Regex101/issues/2289)

8. Add support for quantifying quoted literals [https://github.com/firasdib/Regex101/issues/2293](https://github.com/firasdib/Regex101/issues/2293)

9. Adjust error message for unescaped delimiters [https://github.com/firasdib/Regex101/issues/2286](https://github.com/firasdib/Regex101/issues/2286)

10. Change `twitter` to `X` [https://github.com/firasdib/Regex101/issues/2345](https://github.com/firasdib/Regex101/issues/2345)

11. Fix typo in quickref [https://github.com/firasdib/Regex101/issues/2344](https://github.com/firasdib/Regex101/issues/2344)

12. Add support for version checker construct [https://github.com/firasdib/Regex101/issues/2335](https://github.com/firasdib/Regex101/issues/2335)

13. Upgrade PCRE2 to version 10.44

14. Add support for resizing right sidebar on touch devices [https://github.com/firasdib/Regex101/issues/2330](https://github.com/firasdib/Regex101/issues/2330)

15. Added basic benchmarking feature [https://github.com/firasdib/Regex101/issues/2329](https://github.com/firasdib/Regex101/issues/2329)

16. Add full support for PCRE2 unicode properties [https://github.com/firasdib/Regex101/issues/2336](https://github.com/firasdib/Regex101/issues/2336)

17. Fix issue with viewport calculation and update [https://github.com/firasdib/Regex101/issues/2287](https://github.com/firasdib/Regex101/issues/2287)

# 11.7.0 - 19th of May, 2024

1. Rewrite preview server to improve stability

2. Allow duplicate subpattern names in Golang [https://github.com/firasdib/Regex101/issues/2278](https://github.com/firasdib/Regex101/issues/2278)

3. Fix Library Entry Owners were not able to fork their own expressions

4. Restructured the left sidebar for the regex editor. You now have shortcuts to all the account actions when you are signed in, as well as the regex version selector on the top.

5. Rework settings page to be less cluttered and move help text into hoverable icons

6. Added a match information panel at the bottom of the input fields in the editor, these provide useful info about the caret position and current selection [https://github.com/firasdib/Regex101/issues/1750](https://github.com/firasdib/Regex101/issues/1750)

7. The active page in the left sidebar will now have a more distinct color to highlight the active page

# 11.6.2 - 13th of May, 2024

1. Performance improvements to backend

# 11.6.1 - 12th of May, 2024

1. Behind the scenes updates to ensure stability

# 11.6.0 - 11th of May, 2024

1. Reduce legacy code to ensure compatibility with React 19.

2. Fixed incorrect unicode explanation of tokens in Golang [https://github.com/firasdib/Regex101/issues/2271](https://github.com/firasdib/Regex101/issues/2271)

3. Add more search options to find quantifiers in quickref

4. Fix typo in quickref [https://github.com/firasdib/Regex101/issues/2267](https://github.com/firasdib/Regex101/issues/2267)

5. Add rust specific word boundaries to quickref

6. Change how completed quiz tasks look in the sidebar

# 11.5.3 - 24th of March, 2024

1. Fix parsing of `\\<` and `\\>` in characlasses in Rust

2. Handle parsing bug in Java where character class ranges with spaces while `(?x)` is enabled could cause odd issues

3. Fix parsing of backreferences in PCRE2

# 11.5.2 - 18th of March, 2024

1. Fix issue where server was not correctly identifying assets required for complete page load

2. Include which Rust Regex Crate is used for the Rust Flavor [https://github.com/firasdib/Regex101/issues/2241](https://github.com/firasdib/Regex101/issues/2241)

# 11.5.1 - 10th of March, 2024

1. Add complete support for PCRE2 backreference syntax [https://github.com/firasdib/Regex101/issues/2239](https://github.com/firasdib/Regex101/issues/2239)

2. Ensure single quotes are escaped in JS Code Generator when using the `RegExp` constructor [https://github.com/firasdib/Regex101/issues/2234](https://github.com/firasdib/Regex101/issues/2234)

3. Fix issue where JavaScript flags were incorrectly limited

4. Optimize Whitespace Visualization and bail out of doing so if the string has more than 1500 whitespace [https://github.com/firasdib/Regex101/issues/2231](https://github.com/firasdib/Regex101/issues/2231)

# 11.5.0 - 1st of March, 2024

1. Open newly added unit tests by default

2. Improve tabbing experience in unit test view

3. Improve accessibility of the website for screen readers and other assistive technologies

4. Use the standard keymap in codemirror

5. Reduce bundle size by 20-30% and improve load speeds

6. Upgrade Rust to support the latest syntax [https://github.com/firasdib/Regex101/issues/2167](https://github.com/firasdib/Regex101/issues/2167)

7. Fix "Control character Y" entry in quickref not matching [https://github.com/firasdib/Regex101/issues/2210](https://github.com/firasdib/Regex101/issues/2210)

# 11.4.9 - 8th of February, 2024

1. Fix issue where permalinks would not load [https://github.com/firasdib/Regex101/issues/2224](https://github.com/firasdib/Regex101/issues/2224)

# 11.4.8 - 8th of February, 2024

1. Perform server upgrades and maintenance

2. Update dependencies

3. Fix description of possessive quantifiers [https://github.com/firasdib/Regex101/issues/2184](https://github.com/firasdib/Regex101/issues/2184)

4. Fix delimiters in C# [https://github.com/firasdib/Regex101/issues/2192](https://github.com/firasdib/Regex101/issues/2192)

5. Fix JS octal parser [https://github.com/firasdib/Regex101/issues/2193](https://github.com/firasdib/Regex101/issues/2193)

6. Remove erroneous warning for quantifying lookarounds [https://github.com/firasdib/Regex101/issues/2183](https://github.com/firasdib/Regex101/issues/2183)

7. Update styling of the paginator to be more accessible and readable

8. Improve PWA experience [https://github.com/firasdib/Regex101/issues/2156](https://github.com/firasdib/Regex101/issues/2156)

9. Fix grammatical error [https://github.com/firasdib/Regex101/issues/2197](https://github.com/firasdib/Regex101/issues/2197)

10. Add support for missing flags in the Java flavor [https://github.com/firasdib/Regex101/issues/2206](https://github.com/firasdib/Regex101/issues/2206)

11. Add .NET version to sidebar [https://github.com/firasdib/Regex101/issues/2215](https://github.com/firasdib/Regex101/issues/2215)

12. Fix issue where quiz statistics could say there was a shorter accepted solution than there actually was

# 11.4.7 - 18th of November, 2023

1. Update critical dependencies

# 11.4.6 - 13th of October, 2023

1. Additional DDoS mitigations deployed

2. Simplify some code paths to reduce overall load on server

# 11.4.5 - 11th of October, 2023

1. Ensure the correct status codes are returned to the client

# 11.4.4 - 10th of October, 2023

1. Additional DDoS mitigations in place

2. Fix issue where cache sometimes stored invalid entries

# 11.4.3 - 9th of October, 2023

1. Implement additional DDoS mitigations

# 11.4.1 - 1st of October, 2023

1. Fix animations not working properly

# 11.4.0 - 30th of September, 2023

1. Removed superfluous border above sponsor area

2. Updated dependencies

3. Fix explanation for `[]` in JS (https://github.com/firasdib/Regex101/issues/2154)[https://github.com/firasdib/Regex101/issues/2154]

4. Add additional support for unicode scripts in PCRE2 (https://github.com/firasdib/Regex101/issues/2155)[https://github.com/firasdib/Regex101/issues/2155]

# 11.3.6 - 18th of September, 2023

1. Removed Doppler as sponsor

# 11.3.5 - 3rd of September, 2023

1. Fix `is null` unit test critera not working [https://github.com/firasdib/Regex101/issues/2129](https://github.com/firasdib/Regex101/issues/2129)

2. Fix explanation of whitespace in character classes when `(?xx)` is used [https://github.com/firasdib/Regex101/issues/2133](https://github.com/firasdib/Regex101/issues/2133)

3. Fix group not being highlighted properly in the test string when being clicked in the match info box

4. Added `Export Matches` button to the left sidebar for convenience.

5. Fix issue causing memory leak on backend

6. Fix typos in quickref regarding lookbehinds

7. Fix preview for library not being rendered properly

# 11.3.4 - 17th of August, 2023

1. Added `n` and `xx` flags to the quick reference for PCRE2

2. Fix issue where you could not filter on an individual flavor in the library

3. Quality of Life improvement for the server runtime

# 11.3.3 - 14th of August, 2023

1. Fix issue where CodeMirror would crash when loading certain expressions [https://github.com/firasdib/Regex101/issues/2128](https://github.com/firasdib/Regex101/issues/2128)

# 11.3.2 - 12th of August, 2023

1. Fix typo on settings page

2. Fix quiz response returning incorrect score for shortest solution

3. Fix off-center alignment of highlighted matches

4. Update loading screen design

5. Adjust line height for headers in markdown documents

6. Fix issue where any valid solution in the quiz would overwrite the best solution [https://github.com/firasdib/Regex101/issues/2127](https://github.com/firasdib/Regex101/issues/2127)

7. Add splash screen to ios

# 11.3.1 - 10th of August, 2023

1. Fix "most recent" library order not working

2. Fix link to privacy policy in github repo

3. Update dependencies

# 11.3.0 - 8th of August, 2023

1. Typing `?` in the app while the debugger is in view now opens a list of relevant keyboard shortcuts

2. Fix .net balancing group parser [https://github.com/firasdib/Regex101/issues/2123](https://github.com/firasdib/Regex101/issues/2123)

3. Fix highlights sometimes becoming misaligned [https://github.com/firasdib/Regex101/issues/2051](https://github.com/firasdib/Regex101/issues/2051)

4. Fix javascript code generator using wrong delimiters

5. Reworked the entire preview system to generate nicer, custom, previews of each url.

# 11.2.4 - 2nd of August, 2023

1. Additional optimizations behind the scenes

# 11.2.3 - 2nd of August, 2023

1. Prevent the preview engine from attempting to rendering the debugger or code generator

2. Fix potential overflow of unit test view when tests had very long names

# 11.2.2 - 2nd of August, 2023

1. This update is only for the backend, where performance improvements and minor fixes have been made.

# 11.2.1 - 1st of August, 2023

1. Library authors now automatically upvote their own submission at time of submission

2. Minor tweaks and improvements to the server

# 11.2.0 - 31st of July, 2023

1. Fix issue where debug button was incorrectly made available for unsupported flavors [https://github.com/firasdib/Regex101/issues/2117](https://github.com/firasdib/Regex101/issues/2117)

2. Fix issue where the library details view could overflow on small screens

3. Adjust styling of library entries:

   - Recommended flair now has an icon next to it.
   - On smaller screens, only the icon is shown to preserve space
   - Items are now properly vertically centered
   - Spacing around the different buttons is now even

4. When permalinks are loaded, the selection of the editor is now placed automatically at the end instead of start.

5. Dynamically generate open graph images for preview in [Discord](https://discord.gg/wUA6F6YqSs) and other supported platforms

6. Major rewrite of backend in order to modernize it

# 11.1.2 - 27th of July, 2023

1. Adjust code generator for SED to include all lines in the result [https://github.com/firasdib/Regex101/issues/2116](https://github.com/firasdib/Regex101/issues/2116)

2. Fix issue where a rogue `0` would be visible in the left sidebar on the account page

3. Attempt to fix issue where users would randomly be signed out

4. Ensure flavor label in library details matches the one in the library list

# 11.1.1 - 25th of July, 2023

1. Fix issue where permalinks that should not be editable, could become editable.

# 11.1.0 - 25th of July, 2023

1. Added tooltips to show absolute dates in library view

2. Renamed css variable `--content-alternating-bg` to `--content-inner-bg`

3. Account page has received a face lift:

   - Items are displayed in a visually more pleasing way
   - Patterns are parsed and highlighted as if they were in the main editor
   - The flavor now has the same text as the flavor picker in the regex editor (same goes for library page)
   - Increased size of tags slightly
   - Fix tags potentially overflowing in the left sidebar
   - Ensure long tags are displayed properly on all screen sizes

4. Removed alternating colors in lists to keep layout and information looking consistent

5. The changelog modal would show the `Show All` button before the data was finished loading

6. Added check to ensure tooltips stay within the viewport of the screen

7. Fix regression where you could not save a permalink without a regex string inserted

8. Disable debug button in unit tests when there is no regex input

9. Improve active/inactive visualization of the account page icon in the left sidebar

10. Use the created date when sorting library entries by `Most Recent`

11. Change icon for the `Social` header menu as the previous one could be confused with the `Share` menu in Android

12. Application settings are now replicated to the server, which means you get the same experience everywhere you sign in.

    **Note:** the changes are only replicated to the server after they have been modified in this release or later!

13. Add missing color css variables for new header links for dark mode

# 11.0.5 - 21st of July, 2023

1. Minor visual adjustments:

   - The header is now less cluttered as items are grouped into menus
   - Minor adjustments to colors of selected items in the community regex library
   - Adjust logo position in header to be visually more centered
   - Change the arrow icons on the community page

2. Fix race condition where a vote could be counted multiple times (not persisted, current values are correct)

3. Add support for raw string literals in the .NET flavor

# 11.0.4 - 19th of July, 2023

1. Adjust voting arrow icons on library page to increase clarity

# 11.0.3 - 19th of July, 2023

1. Fix issue where page title was not being updated when navigating between library entries

# 11.0.2 - 19th of July, 2023

1. Minor server optimizations with regards to how Redis is setup

# 11.0.1 - 19th of July, 2023

1. Hotfix for library not loading

# 11.0.0 - 19th of July, 2023

This release reworks major parts of the regex library to make it more performant and provide better features.

1. Regex Community Library changes:

   - The regex library now uses a [binomial proportion confidence interval](https://en.wikipedia.org/wiki/Binomial_proportion_confidence_interval) method for ranking the results

   - Select users of the website are now be given a Community Moderator role on the website. They will be able to perform these additional elevated actions:

     - Flag entries in the regex library as "recommended". These entries will stand out through a different color, and be ranked higher in search results.

     - Remove and edit library submission

     - They will have a flair in their account page that indicates their status

   - Added more sort methods to the community regex library

   - Fix edge case where library item details would unintentionally reappear after having been closed

   - Fix edge case where library would unintentionally make multiple requests for the same data

   - Renamed the Regex Library to Community Library to make it clearer this is maintained by the community

   - Changed default sort for the library page from most recent items to highest ranking

   - Add missing Rust flavor to filters on library page

   - Add informational warning about submissions to the regex library to the submission modal

   - Show when a library entry was last modified

2. Adjust explanation of escaped literals [https://github.com/firasdib/Regex101/issues/2107](https://github.com/firasdib/Regex101/issues/2107)

3. Added more helpful tooltips to disabled menu items to make it clear why they are currently unavailable.

4. Fix C# code generator incorrectly stripping quotes [https://github.com/firasdib/Regex101/issues/2104](https://github.com/firasdib/Regex101/issues/2104)

5. Reduce spacing between unit tests

6. Improve resilience of application to network issues.

   The app will now behave better in cases where the main server is down by still rendering the offline version in the browser.
   It will also handle cases where the API is taking an excessive amount to load, and falls back to the offline cached version.
   The app will inform you through a popup once loaded if it's running offline or not.

   The NGINX timeout has been reduced and mitigations have been put into place to avoid more server outages.

7. Fixed various small typos and issues with the regex quiz.

8. Task 11 (Validate floating point numbers) has now been made optional pending further enhancements.

9. Handle case in regex parser where `(*UCP)` is enabled, but `(*UTF)` is not.

10. Change behavior of save button: if an entry it not modifyable by the user viewing it, it will show a `Fork Regex` button.

    The text has now also changed from `Save Regex` to `Save new Regex` to indicate this is a new entry, and not an update of any existing.

11. Overflowing menu items (that display trailing ...) will now have a native `title` attribute to help display the full text

12. Created a discord server to discuss all things regex, join [here](https://discord.gg/wUA6F6YqSs)!

13. Change the live help button on the left sidebar to open a menu that shows Discord and IRC as two options.

14. Fixed selection menus not closing on click (such as the delimiter menu)

# 10.1.1 - 6th of July, 2023

1. Fix issue where `|` was improperly parsed in character classes in JavaScript

# 10.1.0 - 4th of July, 2023

1. Fix quoted literals causing critical error [https://github.com/firasdib/Regex101/issues/2094](https://github.com/firasdib/Regex101/issues/2094)

2. Added support for the new v-flag in JavaScript [https://github.com/firasdib/Regex101/issues/2074](https://github.com/firasdib/Regex101/issues/2074)

# 10.0.0 - 12th of June, 2023

From this date forth, all entries saved anonymously on the website will have a lifetime of 1 year,
unless accessed within that time period, which will extend their lifetime by another year.

If an entry has not been accessed for a year, it will be automatically removed, starting from the
date of this release. This does **not** apply to entries saved while signed in or those submitted to the library.

**Note: This is not finalized yet, I will review this over the coming year or two and see how things evolve.**

1. Allow hyphens at the end of character classes in Java [https://github.com/firasdib/Regex101/issues/2080](https://github.com/firasdib/Regex101/issues/2080)

2. Remove twitter from the sign in options. If you need to migrate your account, please contact me at contact@regex101.com

3. Add option to control how plain text escapes are explained [https://github.com/firasdib/Regex101/issues/2055](https://github.com/firasdib/Regex101/issues/2055)

4. Allow plain text to be escaped in both GoLang and C# [https://github.com/firasdib/Regex101/issues/2054](https://github.com/firasdib/Regex101/issues/2054)

5. Fix special scenario where highlighted token was not cleared when cursor moved

6. Add tooltip to explain why regex debugger is unavailable [https://github.com/firasdib/Regex101/issues/2078#issuecomment-1591256702](https://github.com/firasdib/Regex101/issues/2078#issuecomment-1591256702)

7. Fix typo where in Javascript regex parser was accepting `\p{Script_Extension=...}` instead of `\p{Script_Extensions=...}`

8. Adjust how surrogate pairs are represented in the regular expression [https://github.com/firasdib/Regex101/issues/2082](https://github.com/firasdib/Regex101/issues/2082)

   When the regex is matching in non-unicode mode, the regex box will show the respective code points being matched -- just as the regex engine treats it.
   This means it might look a little bit funky when you're using the UI, but it's the most accurate representation.

   **Example:**

   `/𐌐?/.test('\ud800')` will match, because the actual regex is `/\ud800\udf10?/`, which is not obvious unless the code points are split up.

   In unicode-mode, i.e., `/𐌐?/u.test('\ud800')`, the regex does not match, and the UI will represent the character differently to reflect that.

9. Improve storage of regexes in the database to avoid encoding errors

# 9.0.8 - 21st of May, 2023

1. Fix crash when inserting a dash (`-`) in Rust outside a character class [https://github.com/firasdib/Regex101/issues/2068](https://github.com/firasdib/Regex101/issues/2068)

# 9.0.7 - 15th of May, 2023

1. Fix regex parsing issue in Rust related to nested character classes and character ranges

2. Fix issue where the substitution result box could grow too large in height

3. Improve resolution scaling for match selector inside regex debugger

# 9.0.6 - 14th of April, 2023

1. Increase contrast of cursor in text editor

2. Fix issue where Rust regex validation would not flag `"#` as an invalid token when `#"` was selected as the delimiter.

3. Fix tab size not working as intended [https://github.com/firasdib/Regex101/issues/2044](https://github.com/firasdib/Regex101/issues/2044)

4. Fix editor tooltips in test area not working properly with certain unicode characters

# 9.0.5 - 12th of April, 2023

1. Added validation to limit amount of groups that can be nested

2. Fix issue where query parameters in library and account page did not remain after switching page

# 9.0.4 - 5th of April, 2023

1. Fix issue where cursor was not always visible when at the start of the line in Firefox

2. Add initial RTL support. This is limited for many reasons, partially because of CodeMirror,
   but also because the general assumption is the engine matches LTR, but visually things are RTL.

3. Improve unicode script validation in Rust

4. Add missing quickref entries [https://github.com/firasdib/Regex101/issues/1963](https://github.com/firasdib/Regex101/issues/1963)

5. Fix wrong placeholder text [https://github.com/firasdib/Regex101/issues/2036](https://github.com/firasdib/Regex101/issues/2036)

6. Fix issue where Golang would not properly identify non-participating groups

7. Fix crash in python flavor when inserting pipe character [https://github.com/firasdib/Regex101/issues/2038](https://github.com/firasdib/Regex101/issues/2038)

8. Fix parsing of surrogate values in Rust

# 9.0.3 - 5th of April, 2023

1. Fix display of delimiters in the UI for Rust

2. Adjust color of delimiters in explanation UI

3. Ensure Rust respects the correct delimiter set in the UI when matching [https://github.com/firasdib/Regex101/issues/2034](https://github.com/firasdib/Regex101/issues/2034)

4. Fix parsing of character classes with comments in them in Rust

5. Disallow backreferences/octals in Rust

6. Fix validation of character ranges in char classes for

7. Fix explanation of plain text containing whitespace when x-mode is enabled for Rust

# 9.0.2 - 3rd of April, 2023

1. Fix display of delimiters for Rust

2. Fix issue with deleting entire regex tree through regex modal

# 9.0.1 - 3rd of April, 2023

1. Fix issue in parsing opening braces in Rust

2. Fix issue where widgets in CodeMirror were not highlighted when hovered

3. Change line separator option to be opt in. Using the default `Automatic` setting will preserve the old expected behavior.

4. Fix issue where version delete URL was not always presented back to the user

5. Fix issue where delete URL was incorrectly generated on the client

6. Fix issue where you could not update a permalink where no regex was input

7. Fix issue where deleted items were not always immediately cleared from the cache

# 9.0.0 - 3rd of April, 2023

This is a major release that includes the brand new [CodeMirror 6](https://codemirror.net/).
This editor is the latest version which includes numerous bug fixes from
the previous version, but also quite likely, some new ones.

Please report any and all oddities you encounter in the editor.

1. Upgrade CodeMirror to version 6

   - Completely rewritten all editors
   - Improved performance tremendously
   - Fixed many of the quirks in the previous editor, such as newline visualization, match hover, etc.
   - Better visualize non-printable characters in the document
   - Added support for custom line separators in the document
   - Fix edge cases where hovering match results did not always produce a tooltip
   - Removed auto complete brackets option
   - Clicking a match in the Match Information box will highlight the string in the editor using native selection
   - Rewrite editor tooltips to be more efficient
   - Better accessibility
   - Improved clarity of selected tokens in regex input

2. Fix automatic code generator mode not working as intended [https://github.com/firasdib/Regex101/issues/2002](https://github.com/firasdib/Regex101/issues/2002)

3. Make text area for unit test allow tab to be inserted [https://github.com/firasdib/Regex101/issues/2001](https://github.com/firasdib/Regex101/issues/2001)

4. Show whitespace in unit test description [https://github.com/firasdib/Regex101/issues/2004](https://github.com/firasdib/Regex101/issues/2004)

5. Move version menu to the right of match indicator to avoid layout shifts

6. Limit version menu to half the height from before

7. Fix match info not loading when scrolling when sidebar was collapsed

8. Added ability for users to delete individual regex versions

9. Change wording of empty matches [https://github.com/firasdib/Regex101/issues/2008](https://github.com/firasdib/Regex101/issues/2008)

10. Fix `a` flag not working in Python flavor [https://github.com/firasdib/Regex101/issues/2003](https://github.com/firasdib/Regex101/issues/2003)

11. Fix unit tests always passing in .NET when groups did not participate in the match

12. Remove warning about the usage of named capture groups in JavaScript as support is now at >95% across all browsers [https://github.com/firasdib/Regex101/issues/2005](https://github.com/firasdib/Regex101/issues/2005)

13. Minor bug fixes to task and test descriptions in the regex quiz

14. The `UCP` verb in PCRE will now reflect changes in the explanation tab accordingly

15. Fix explanations not taking Unicode Matching in Java into account [https://github.com/firasdib/Regex101/issues/2022](https://github.com/firasdib/Regex101/issues/2022)

16. Improve performance of regex explainer slightly

17. Improve explanations of character class intersection/subtraction et. al.

18. Added an entry for conditional replacements to the quickref for PCRE2

19. Add support for Rust! Huge thanks to [@tgross35](https://github.com/tgross35)! [https://github.com/firasdib/Regex101/issues/1208](https://github.com/firasdib/Regex101/issues/1208)

20. Fix issue where `\0` was explained incorrectly in JavaScript

21. Fix issue where when trying to explain certain characters the site would lock up due to an inifite loop

22. Golang will now report back the correct UTF-8 indices in the UI, instead of the adjusted UTF-16 ones.

23. Add support for saving permalinks without regex [https://github.com/firasdib/Regex101/issues/2032](https://github.com/firasdib/Regex101/issues/2032)

24. Updated paypal donation link to their new format

# 8.4.10 - 12th of February, 2023

1. Fix some tokens incorrectly treated as octal escapes in Python substitutions [https://github.com/firasdib/Regex101/issues/1987](https://github.com/firasdib/Regex101/issues/1987)

2. Fix issue where octal escapes inside character classes were identified as backreferences in javascript [https://github.com/firasdib/Regex101/issues/1992](https://github.com/firasdib/Regex101/issues/1992)

# 8.4.9 - 5th of January, 2023

1. Fix character range validation in Java when using the vertical tab shorthand

2. Improve UX around save modal to reduce confusion w.r.t if the data is saved or not [https://github.com/firasdib/Regex101/issues/1948](https://github.com/firasdib/Regex101/issues/1948)

3. Update PCRE2 to version 10.42

4. Add more details to `flavors.md` document

5. Added buttons in regex debugger to step one step forwards/backwards and adjusted the default step limit to 1000 steps [https://github.com/firasdib/Regex101/issues/1788](https://github.com/firasdib/Regex101/issues/1788)

6. Fix issue in .NET where meta sequences would incorrectly flag pattern as invalid when paired with ranges in character classes [https://github.com/firasdib/Regex101/issues/1969](https://github.com/firasdib/Regex101/issues/1969)

7. Added support for `\N{U+hh..}` syntax for PCRE2 [https://github.com/firasdib/Regex101/issues/1967](https://github.com/firasdib/Regex101/issues/1967)

# 8.4.8 - 12th of December, 2022

1. Fix issue with `null` strings causing match errors

# 8.4.6 - 11th of December, 2022

1. Adjusted regex parser to flag specific constructs as incompatible with .NET `NonBacktracking` mode

# 8.4.5 - 10th of December, 2022

1. Add `color-scheme` to dark/light themes [https://github.com/firasdib/Regex101/issues/1945](https://github.com/firasdib/Regex101/issues/1945)

2. Add support for `RegexOptions.NoBacktracking` in .NET 7 [https://github.com/firasdib/Regex101/issues/1951](https://github.com/firasdib/Regex101/issues/1951)

3. Change quote style for PHP generated code for substitution text [https://github.com/firasdib/Regex101/issues/1950](https://github.com/firasdib/Regex101/issues/1950)

4. Add support for `(*UTF)` verb shorthand. See [https://github.com/firasdib/Regex101/issues/1903](https://github.com/firasdib/Regex101/issues/1903).

# 8.4.4 - 16th of November, 2022

1. Fix issue where older safari versions would crash on page load [https://github.com/firasdib/Regex101/issues/1941](https://github.com/firasdib/Regex101/issues/1941)

# 8.4.3 - 13th of October, 2022

1. Fix numerous issues related to verbs [https://github.com/firasdib/Regex101/issues/1923](https://github.com/firasdib/Regex101/issues/1923)

   - Add support for `${*MARK}` and `$*MARK` in PCRE2 substitutions
   - Fix explanation for verbs
   - Fix pattern parsing to allow verbs with any name

# 8.4.2 - 12th of October, 2022

1. Added a "Show all" button to the whats new modal since the document is getting quite large.

2. Fixed int32 overflow for subpatterns in .NET

3. Added more tests to floating point task to avoid patterns allowing numbers such as `+2+5`

4. Fixed error when defining octals in JS [https://github.com/firasdib/Regex101/issues/1922](https://github.com/firasdib/Regex101/issues/1922)

# 8.4.1 - 25th of September, 2022

1. Reduce motion now reduces motion like OSX

# 8.4.0 - 25th of September, 2022

1. Change url for noscript tag

2. Fix issue in javascript when parsing ambiguous octal escapes/backreferences [https://github.com/firasdib/Regex101/issues/1899](https://github.com/firasdib/Regex101/issues/1899)

3. Improve explanations for shorthands in .NET and for zero-width matches [https://github.com/firasdib/Regex101/issues/1891](https://github.com/firasdib/Regex101/issues/1891)

4. Save all fields when saving/updating a regex, even if they are currently not visible in the editor [https://github.com/firasdib/Regex101/issues/1889](https://github.com/firasdib/Regex101/issues/1889)

5. Update setting to enable steps to reflect it only works in supported flavors [https://github.com/firasdib/Regex101/issues/1890](https://github.com/firasdib/Regex101/issues/1890)

6. Add support for conditional references being defined at any point in the pattern [https://github.com/firasdib/Regex101/issues/1900](https://github.com/firasdib/Regex101/issues/1900)

7. Upgrade .NET 7 to RC1

8. Improve quickref search [https://github.com/firasdib/Regex101/issues/1876](https://github.com/firasdib/Regex101/issues/1876)

9. Improve quickref with regards to lazy quantifiers [https://github.com/firasdib/Regex101/issues/1874](https://github.com/firasdib/Regex101/issues/1874)

10. Add support for reduce motion API

# 8.3.11 - 31st of August, 2022

1. Added .ENV as sponsor to the website

2. Fixed specific scenario in Java where character class ranges could throw errors when combined with free spacing mode

# 8.3.10 - 19th of August, 2022

1. Fix substitution not working when `""` was used in the regex [https://github.com/firasdib/Regex101/issues/1870](https://github.com/firasdib/Regex101/issues/1870)

2. Escape quotes in the code generator for .NET [https://github.com/firasdib/Regex101/issues/1875](https://github.com/firasdib/Regex101/issues/1875)

# 8.3.9 - 12th of August, 2022

1. Fix issue where unit tests targetting specific groups always passed [https://github.com/firasdib/Regex101/issues/1863](https://github.com/firasdib/Regex101/issues/1863)

# 8.3.8 - 11th of August, 2022

1. Improve performance on mobile platforms by pre-rendering it on the server

# 8.3.7 - 10th of August, 2022

1. Defer loading of external, non-critical assets, to improve page loading speed

# 8.3.6 - 9th of August, 2022

1. Fix tooltips lagging due to React batching UI updates

2. Fix issue in .NET where unit tests would not allow you to select named groups [https://github.com/firasdib/Regex101/issues/1861](https://github.com/firasdib/Regex101/issues/1861)

3. Fix issue where unit tests would not automatically re-run after pattern errors were corrected

# 8.3.5 - 4th of August, 2022

1. Adjust Sentry to only collect non-console errors

# 8.3.4 - 3rd of August, 2022

1. Fix tabs not being visualized correctly [https://github.com/firasdib/Regex101/issues/1857](https://github.com/firasdib/Regex101/issues/1857)

2. Fix regression in capture group validation

3. Adjust escaped literal validation for JavaScript when in substitution mode

4. Fix keyboard shortcuts not working when sidebar is collapsed

# 8.3.3 - 30th of July, 2022

1. Fix numeric references to named groups in substitution for .NET [https://github.com/firasdib/Regex101/issues/1853](https://github.com/firasdib/Regex101/issues/1853)

# 8.3.2 - 25th of July, 2022

1. Fix popups sometimes appearing outside the visible viewport

# 8.3.1 - 25th of July, 2022

1. Fix escaped quotes not being matched in .NET

2. Fix first task not being enabled for new users [https://github.com/firasdib/Regex101/issues/1851](https://github.com/firasdib/Regex101/issues/1851)

## 8.3.0 - 24th of July, 2022

1. Fix hyphen not being escapeable inside charcter classes in Javascript when u-flag was enabled

2. Improve message description when browser validation fails

3. Fix case where ranges with octal escapes were improperly validated in the PCRE flavor

4. Updated multiple dependencies to the latest

5. Fix parsing of modifier reset groups

6. Fix named groups in .NET sometimes not validated properly

7. Fix handling of whitespace in character classes when in free-spacing mode in Java flavor

8. Fix parsing of redefined named subpatterns in .NET

9. Fix validation of subpattern names in .NET

10. Brighten third match colors in dark mode [https://github.com/firasdib/Regex101/issues/1823](https://github.com/firasdib/Regex101/issues/1823)

11. Fix hamburger icon sometimes appearing on top of logo [https://github.com/firasdib/Regex101/issues/1819](https://github.com/firasdib/Regex101/issues/1819)

12. Fix incorrect alternative notation in quickref entry for named groups in Java [https://github.com/firasdib/Regex101/issues/1804](https://github.com/firasdib/Regex101/issues/1804)

13. Change .NET delimiter to visually show `@"..."` [https://github.com/firasdib/Regex101/issues/1842](https://github.com/firasdib/Regex101/issues/1842)

14. Fix "rave fest" when printing the page on OSX in Chrome [https://github.com/firasdib/Regex101/issues/1817](https://github.com/firasdib/Regex101/issues/1817)

15. Default to showing the library title (if any) in the account page for entries that have no titles [https://github.com/firasdib/Regex101/issues/1794](https://github.com/firasdib/Regex101/issues/1794)

16. Allow signed in users to add library entries to their favorites from the library page directly [https://github.com/firasdib/Regex101/issues/1794](https://github.com/firasdib/Regex101/issues/1794)

17. Highlighted tokens are no longer cleared when scrolling in the regex editor [https://github.com/firasdib/Regex101/issues/1847](https://github.com/firasdib/Regex101/issues/1847)

## 8.2.0 - 1st of May, 2022

1. Fix spelling of Portuguese [https://github.com/firasdib/Regex101/issues/1776](https://github.com/firasdib/Regex101/issues/1776)

2. Fix regex matches not always sized properly [https://github.com/firasdib/Regex101/issues/1777](https://github.com/firasdib/Regex101/issues/1777)

3. Fix edge cases in .NET matching

   - [https://github.com/firasdib/Regex101/issues/1737](https://github.com/firasdib/Regex101/issues/1737)
   - [https://github.com/firasdib/Regex101/issues/1760](https://github.com/firasdib/Regex101/issues/1760)

4. Added note about Edge and Web Assembly not playing nicely in certain scenarios

## 8.1.3 - 7th of April, 2022

1. Fix lookahead explanation incorrectly saying lookbehind (and vice versa) [https://github.com/firasdib/Regex101/issues/1768](https://github.com/firasdib/Regex101/issues/1768)

2. Fix unit tests crashing in Python flavor [https://github.com/firasdib/Regex101/issues/1770](https://github.com/firasdib/Regex101/issues/1770)

## 8.1.2 - 25th of March, 2022

1. Fix issue where focus was not maintained within menus

2. Fix incorrect explanation of negative lookbehinds [https://github.com/firasdib/Regex101/issues/1757](https://github.com/firasdib/Regex101/issues/1757)

3. Fix validation for incomplete hex escapes in javascript substitution mode

4. Fix issue where flags were not correctly interpreted in pattern in certain scenarios

5. The JavaScript code generator will now always include the `new RegExp` syntax for ease of copy

## 8.1.1 - 24th of March, 2022

1. Fix issue where relative conditionals were not properly validated for PCRE

2. Fix issue where backreferences in Javascript under specific circumstances caused crashes

## 8.1.0 - 23rd of March, 2022

1. Reduce amount of files precached by service worker

   This is to reduce the bandwidth usage and cost. The files will be cached on an as-you-go basis instead.

   If you intend to run the application offline, you'll have to first load the flavors (and functions) you want to cache locally.
   After you have done this, the flavor will continue to function offline permanently.

2. Fix miscellaneous parser bugs:

   1. Fix bug where character range validation would fail in Javascript mode
   2. Fix validation of alternatives within conditionals
   3. Fix issue where non-atomic lookbehinds were not validated accurately in PCRE2
   4. Ensure conditional conditions cannot be quantified
   5. Substitution parser was not validating edge cases in Java and Javascript properly (due to typo)
   6. Fix long octal escapes `\o{}` causing crashes [https://github.com/firasdib/Regex101/issues/1754](https://github.com/firasdib/Regex101/issues/1754)
   7. Fix conditionals in python causing crashes [https://github.com/firasdib/Regex101/issues/1752](https://github.com/firasdib/Regex101/issues/1752)
   8. Fix issue where .NET crashes when using inline modifiers in the root of a conditional. The site will now handle it and throw an error.

3. Fix edge case where tooltip would not accurately reflect token under cursor

4. Added warnings when using JS constructs that might not be supported in all browsers

5. The parsers will now parse using char codes or code points depending on if unicode is enabled or not

## 8.0.3 - 20th of March, 2022

1. Disable unnecessary events being sent to Sentry

## 8.0.2 - 20th of March, 2022

1. Switch to lightweight analytics platform plausible

## 8.0.1 - 20th of March, 2022

1. Fix substitution mode not working for PCRE, Python and Go

2. Fix parser bug causing app to crash

## 8.0.0 - 20th of March, 2022

1. Complete rewrite of the regex parser to accommodate new features

   - Improved performance by 10x
   - Simplified code base
   - Made parser more easily extensible for future flavors
   - Reduced bundle footprint

2. Fixed numerous parser bugs:

   - Braces are now allowed inside character classes in Javascript [https://github.com/firasdib/Regex101/issues/1742](https://github.com/firasdib/Regex101/issues/1742)
   - Verbs are properly handled at start of regex for both PCRE and PCRE2 [https://github.com/firasdib/Regex101/issues/1740](https://github.com/firasdib/Regex101/issues/1740)
   - Fixed issue with .NET and implicit lookaheads inside conditionals

3. Improved performance of tooltips when working with large documents

4. Fixed explanation of plain text when free spacing mode is enabled

5. Lists with repeated characters will not be explained multiple times unnecessarily

6. Removed dependency on dotall flag to allow older browsers to function

7. Permalinks will now be redirected to the latest version if the version number is omitted

## 7.1.7 - 7th of March, 2022

1. Fix quotes not being escaped properly in .NET code generator for substitution text

## 7.1.6 - 3rd of March, 2022

1. Adjust generated code for .NET [https://github.com/firasdib/Regex101/issues/1734](https://github.com/firasdib/Regex101/issues/1734)

2. Fix match error in .NET in certain scenarios [https://github.com/dotnet/runtime/issues/66212](https://github.com/dotnet/runtime/issues/66212)

3. Fix parsing of conditional statements in .NET flavor

4. Fix parsing of control codes in .NET

## 7.1.5 - 2nd of March, 2022

1. Added explanation to missing substitution tokens in .NET

## 7.1.4 - 2nd of March, 2022

1. Ensure .NET balancing groups can be quantified [https://github.com/firasdib/Regex101/issues/1730](https://github.com/firasdib/Regex101/issues/1730)

2. Fix edge case in `\c` construct for javascript

## 7.1.2 - 1st of March, 2022

1. Fix service worker reload loop issue

2. Improve initial load times of .NET

## 7.1.0 - 28th of February, 2022

1. Add missing .NET filter to regex library page

2. Add support for named backreference using `\k'name'` syntax

3. Add support for undocumented backreference syntax using `\<name>` and `\'name'`

4. Add support for modifier reset syntax in PCRE2 [https://github.com/firasdib/Regex101/issues/1728](https://github.com/firasdib/Regex101/issues/1728)

5. Added support for character class subtraction in .NET

6. Add explicit information about callout support in the parser/explanation [https://github.com/firasdib/Regex101/issues/1729](https://github.com/firasdib/Regex101/issues/1729)

## 7.0.2 - 26th of February, 2022

1. Adjust escaped literal parser for .NET to handle edge cases

2. Ensure tooltip shows sub-captures for .NET flavor

## 7.0.1 - 26th of February, 2022

1. Fixed .NET to allow variable width lookbehinds

2. Add support for multiple group captures in .NET

3. Added support for RTL matching in .NET

## 7.0.0 - 26th of February, 2022

1. Minor tweaks to UI

2. Improve quickref

   1. Fix recursion example [https://github.com/firasdib/Regex101/issues/1714](https://github.com/firasdib/Regex101/issues/1714)
   2. Update explanation and quickref docs to be more accurate when explaning subroutine calls [https://github.com/firasdib/Regex101/issues/1601](https://github.com/firasdib/Regex101/issues/1601)
   3. Improve explanation and examples of `\Z` [https://github.com/firasdib/Regex101/issues/1691](https://github.com/firasdib/Regex101/issues/1691)

3. Update golang to the latest version, fixes [https://github.com/firasdib/Regex101/issues/1588](https://github.com/firasdib/Regex101/issues/1588)

4. Improve performance of golang implementation

5. Upgrade PCRE2 to version 10.39

6. Reduce usage of deprecated `findDOMNode`

7. Add support to .NET [https://github.com/firasdib/Regex101/issues/156](https://github.com/firasdib/Regex101/issues/156)

   Huge thanks to [Alberto Monteiro](https://github.com/AlbertoMonteiro) for his help in making this possible.

8. Show metadata for failed matches (steps and time taken)

9. Improve error for Posix Word Boundaries in non-PCRE flavors [https://github.com/firasdib/Regex101/issues/1722](https://github.com/firasdib/Regex101/issues/1722)

10. Improve Swift code generation [https://github.com/firasdib/Regex101/issues/1678](https://github.com/firasdib/Regex101/issues/1678)

11. Align ECMAScript caret notation parser with official specification

12. Fix errors in verb parsing and improve explanations [https://github.com/firasdib/Regex101/issues/1724](https://github.com/firasdib/Regex101/issues/1724)

## 6.3.8 - 1st of February, 2022

1. Fix edge case issue with javascript substitution parser

2. Fix parsing of character class ranges with quoted literals

## 6.3.7 - 29th of January, 2022

1. Disallow character ranges with shorthand escape sequences in javascript

2. Adjust border color of highlighted match in test string

3. Reduced bundle size even more

4. Updated server to the latest and greatest to ensure regex101 can continue to work for many years to come

5. Added brotli compression to save on load times and bandwidth

## 6.3.6 - 27th of January, 2022

1. Adjust nginx config, minor quality of life adjustments for performance

## 6.3.5 - 26th of January, 2022

1. Fix match artifacts sometimes appearing when pasting text in the test input

2. Improve performance and positional calculation of tooltips

## 6.3.4 - 25th of January, 2022

1. Fix issue where match highlights were sometimes incorrect

2. Fix issue where line numbers sometimes caused match highlights to be misaligned

3. Additional internal performance tweaks

## 6.3.3 - 24th of January, 2022

1. Fix unit test state sometimes going out of sync with the UI

2. Avoid editor tooltips going out of screen

## 6.3.2 - 23rd of January, 2022

1. Fix parsing of Posix Classes [https://github.com/firasdib/Regex101/issues/1707](https://github.com/firasdib/Regex101/issues/1707)

## 6.3.1 - 23rd of January, 2022

1. Avoid computing match information that is not yet visible on screen to improve performance

## 6.3.0 - 22nd of January, 2022

1. Performance improvements

   These changes might introduce new bugs or regressions, due to the complex nature of the website and its functionality.
   If you do notice any inconsistencies, please create an issue at [https://github.com/firasdib/Regex101/issues/](https://github.com/firasdib/Regex101/issues/). Thank you.

   - Fix CPU hog when deleting text in the test input
   - Skip non-participating groups from paint logic
   - Improve debounce logic for async worker creation when handling complex patterns/input

2. Fix issue where some errors slipped through when switching flavors

## 6.2.7 - 22nd of January, 2022

1. Fix issue where painted items sometimes got out of sync when scrolling rapidly

2. Remove old match information if it is outdated for a prolonged amount of time.
   This will mainly affect slow machines, those working with large amounts of information or slow regular expressions.

## 6.2.6 - 21st of January, 2022

1. Fix issue where regex input sometimes became unresponsive [https://github.com/firasdib/Regex101/issues/1705](https://github.com/firasdib/Regex101/issues/1705)

## 6.2.5 - 20th of January, 2022

1. Update link to Doppler sponsor

2. Background maintenance work, updating dependencies, etc.

## 6.2.4 - 17th of January, 2022

1. Experiment with lazy loading sentry at page load for better error reporting

## 6.2.3 - 16th of January, 2022

1. Improve animation smoothness of menus

2. Add shortcut to show all unit test if filtered results returned empty set

## 6.2.2 - 15th of January, 2022

1. Fix issue where menus were appearing out of screen [https://github.com/firasdib/Regex101/issues/1701](https://github.com/firasdib/Regex101/issues/1701)

## 6.2.1 - 14th of January, 2022

1. Fix issue with tooltips not always appearing properly

## 6.2.0 - 14th of January, 2022

1. Reduced bundle size even further

2. Improved performance of regex parser

3. Fixed some animations causing irregular stutter

4. Fixed memory leak

## 6.1.7 - 12th of January, 2022

1. Fix JS edge case w.r.t `\c` in character classes

## 6.1.6 - 11th of January, 2022

1. Add filters to unit test view through a menu [https://github.com/firasdib/Regex101/issues/1697](https://github.com/firasdib/Regex101/issues/1697)

2. Fix issue where unit test status was not properly displayed in the header [https://github.com/firasdib/Regex101/issues/1696](https://github.com/firasdib/Regex101/issues/1696)

## 6.1.5 - 10th of January, 2022

1. Fix `ctrl+shift+s` shortcut when there was nothing to save

2. Fix issue where tooltips would sometimes stop showing after closing a modal or sidebar

3. Added new flavor guide with some initial information. This document will be updated and improved with time.

## 6.1.4 - 6th of January, 2022

1. Add skeleton loader to ease jumping of sponsor block when page loads

## 6.1.3 - 5th of January, 2022

1. Fix library entries fetching unnecessarily

2. Fix submit to library modal not showing the correct links after submitting an entry

## 6.1.2 - 29th of December, 2021

1. Minor fixes here and there

2. Added link to [r101.cf](https://r101.cf) for translations

3. Improve server performance

## 6.1.1 - 22nd of December, 2021

1. Add information modal around ads and privacy

## 6.1.0 - 21st of December, 2021

1. Only render shortcuts when they are enabled to avoid any confusion

## 6.0.1 - 21st of December, 2021

1. Fixed escaping issue when populating the initial state on the server

## 6.0.0 - 20th of December, 2021

1. This release does not add any major functionality for you users, but has completely changed things behind the scenes.
   All dependencies are now up to date, and the build system has been revamped. I've cleaned up a lot of things too.

2. Improved performance - bundle size reduced by over 20%

3. Delete link in the sidebar can now be copied (right click -> copy link)

4. The site can now be themed by users (using css variables)

5. Unit tests can now be individually debugged in the PCRE flavors

6. Zero width matches are now painted last to ensure they are always visible [https://github.com/firasdib/Regex101/issues/1653](https://github.com/firasdib/Regex101/issues/1653).

7. Fixed numerous issues with the quickref

   - [https://github.com/firasdib/Regex101/issues/1566](https://github.com/firasdib/Regex101/issues/1566)
   - [https://github.com/firasdib/Regex101/issues/1679](https://github.com/firasdib/Regex101/issues/1679)
   - [https://github.com/firasdib/Regex101/issues/1665](https://github.com/firasdib/Regex101/issues/1665)
   - [https://github.com/firasdib/Regex101/issues/1637](https://github.com/firasdib/Regex101/issues/1637)
   - [https://github.com/firasdib/Regex101/issues/1681](https://github.com/firasdib/Regex101/issues/1681)

8. Null matches are now explained as such in the match info pane

9. Fix issue where matches were painted incorrectly after resizing website

10. Maintain scroll position in the substitution box when adjusting test string or regex

11. Fix handling of `\v` in Python flavor [https://github.com/firasdib/Regex101/issues/1676](https://github.com/firasdib/Regex101/issues/1676)

12. Editor is now forced to work LTR to ensure consistency between regex matcher and indices [https://github.com/firasdib/Regex101/issues/1576](https://github.com/firasdib/Regex101/issues/1576)

13. Reworked look and feel of fullscreen modal (used when generating code samples, etc).

14. Editor tooltips will now hide themselves when you're selecting text

15. Added ability to disable keyboard shortcuts [https://github.com/firasdib/Regex101/issues/1646](https://github.com/firasdib/Regex101/issues/1646)

16. Rewritten large parts of the backend to improve performance and page speed

## 5.17.0 - 5th of November, 2021

1. Added ability to load examples from the quickref.

   Do note that they will overwrite the content in the inputs,
   but you can undo it by using ctrl+z

2. Improved performance of regex editor

   - Improved the efficiency of the matches being painted on the screen
   - Added dynamic mechanism to detect when regex matching is falling behind input speed

3. Fixed issue where elements highlighted by hovering were not always cleared

## 5.16.2 - 10th of October, 2021

1. Improved server application performance.

   Analyzed db performance using [eversql.com](https://eversql.com).
   Thank you Tomer!

   Hopefully you will experience a quicker regex library and website over all!

2. Fix issue where highlighted matches would sometimes get "stuck" after hovering

3. Remove dependency on transparent canvas

   This might improve performance, it might have no noticeable difference.

4. Fix edge cases where canvas could appear janky

## 5.16.1 - 10th of October, 2021

1. Fix regression when painting match results on canvas (thanks digitok for reporting)

## 5.16.0 - 8th of October, 2021

1. Add support for named backreferences in JS substitution mode. See [https://github.com/firasdib/Regex101/issues/1652](https://github.com/firasdib/Regex101/issues/1652)

2. Fix parsing of escaped dollar signs in JS substitution mode.

3. Add tests to task 15. See [https://github.com/firasdib/Regex101/issues/1645](https://github.com/firasdib/Regex101/issues/1645)

## 5.15.3 - 8th of October, 2021

1. Improve error handling of recursion related errors

2. Improve handling of escaped text literals and unicode

3. Update codemirror to latest version

4. Updated translations

5. Improved handling of links in the header on smaller screens

## 5.15.0 - 22nd of September, 2021

1. Added support for new `d` flag in JavaScript

## 5.14.1 - 3rd of September, 2021

1. Fix collating posix class parsing

2. Ensure `performance` is polyfilled properly

## 5.14.0 - 9th of August, 2021

1. Slightly darken theme color for the light theme

2. Add new option to disable the default tabbing behavior.

   This options allows you to decide what should happen when you hit the tab key:

   1. Switch to the next field in the document (default)

   2. Consume the tab key and insert a tab character

3. Fix explanation of `\P`

## 5.13.6 - 31st of July, 2021

1. Add separate meta descriptions for the different sub pages

2. Fix tooltip direction switching randomly in the account page

3. Improve error handling when `\C` is used

4. Fix character range check for surrogate pairs

## 5.13.5 - 26th of July, 2021

1. Copy behavior of Perl and disallow \K inside lookbehinds in PCRE. See [https://bugs.exim.org/show_bug.cgi?id=2792](https://bugs.exim.org/show_bug.cgi?id=2792)

2. Fix minor issues with lookbehind length calculation in edge case scenarios

3. Update quote token color in dark theme

## 5.13.4 - 18th of July, 2021

1. Fix issue where the scroll bar was unnecessarily shown for library entries

2. Fix issue where page sometimes became non-interactable [https://github.com/firasdib/Regex101/issues/1618](https://github.com/firasdib/Regex101/issues/1618)

## 5.13.3 - 13th of July, 2021

1. Format large numbers to make them easier to read

2. Code generator button is now disabled when in List Substitution mode to avoid confusion

3. Fix posix class parser for PCRE and PCRE2

## 5.13.2 - 11th of July, 2021

1. Added tooltip to match indicator when unhandled errors are encountered (hover to view)

2. Fix explanation of `\Q...\E` [https://github.com/firasdib/Regex101/issues/1614](https://github.com/firasdib/Regex101/issues/1614)

## 5.13.1 - 10th of July, 2021

1. Plain text explanation now shows code points in decimal, hex and octal

   The explanation is collapsed by default to avoid creating too much noise.

2. Plain text in the substitution box is now explained in a similar fashion to the regex input

3. Adjusted styling and timing of tooltips

   - Timing of tooltips has been adjusted slightly, they now trigger faster
   - A drop shadow has been added to give them a bit of depth
   - The closing animation for tooltips were broken, its now fixed
   - Performance of tooltips has been improved slightly by using composite layers in the browser

## 5.13.0 - 7th of July, 2021

1. Fix regex parsing of relative subpattern references

2. Handle error caused by nesting too many conditional replacements in PCRE2

3. Disallow null bytes in regex

4. Use high precision timers for calculating computational time spent in regex

5. Update favicon and add more PWA support

## 5.12.3 - 6th of July, 2021

1. Fix java subst pattern parsing (hopefully once and for all)

2. Fix subst conditional coloring not repeating properly

3. Reworked substitution area to be more efficient. If you encounter any odd behavior, please report it as a bug on github.

## 5.12.2 - 5th of July, 2021

1. Improve paste performance further

2. Fix issue with Java code generator [https://github.com/firasdib/Regex101/issues/1611](https://github.com/firasdib/Regex101/issues/1611)

3. Remove the `2.7` part from the python flavor text

4. Improved performance on initial page load

## 5.12.1 - 1st of July, 2021

1. Fix issue with `\Q...\E` when pasting regexes into the regex box (Thanks digitok)

2. Disallow `\C` in lookbehinds in PCRE when enabling UTF16 mode

3. Error if user places unescaped `{` inside conditionals in PCRE mode during substitution

4. Fix numeric escapes sometimes not working in java substitution mode

5. Update codemirror to latest version

6. Fix lookbehind length calculation in x-mode

7. Add proper surrogate pair parsing for java flavor

## 5.12.0 - 25th of June, 2021

1. Fixed typo in quickref for charclass intersection [https://github.com/firasdib/Regex101/issues/1598](https://github.com/firasdib/Regex101/issues/1598)

2. Add support for `LD` unicode script in Java [https://github.com/firasdib/Regex101/issues/1590](https://github.com/firasdib/Regex101/issues/1590)

3. Fix issue where relative backreferences could reference invalid groups

4. Fixed issue where nested branch reset groups would not validate properly

5. Added indicator for zero width character matches [https://github.com/firasdib/Regex101/issues/1593](https://github.com/firasdib/Regex101/issues/1593)

6. Generate error when `\E` is encountered without a corresponding `\Q`

7. Fix edge case in inline modifier parsing for Java flavor

8. Disallow quantifiers inside lookbehinds for Python flavor

9. Fix issue where unknown unicode categories were accepted for Java

## 5.11.3 - 23rd of June, 2021

1. Fix potential race condition when initially loading the page

2. Add word-wrapping to user submitted descriptions to avoid page overflow issues

## 5.11.2 - 11th of June, 2021

1. Fix issue where quantifiers on certain tokens did not visually show up in explanation

## 5.11.0 - Xth of May, 2021

1. Fixed issue where `\8` and `\9` would not work in Java substitution strings

2. Updated IRC link to Libera

## 5.10.0 - 12th of May, 2021

1. Fixed general unicode category for Java [https://github.com/firasdib/Regex101/issues/1570](https://github.com/firasdib/Regex101/issues/1570)

2. Added new delimiters to javascript flavor

3. Added highlight in regex input when clicking a group in the match info pane

4. Emphasize negative unit tests with an underline

5. Added nbsp to explanation for `\s` for python flavor

## 5.9.0 - 19th of April, 2021

1. Added ability to delete your account

## 5.8.0 - 10th of April, 2021

1. Added support for all verbs in PCRE2

2. Fixed parsing of inline modifiers in golang [https://github.com/firasdib/Regex101/issues/1551](https://github.com/firasdib/Regex101/issues/1551)

3. Fix library url after uploading entry

4. Fix "My Library Entries" showing favorited entries

5. Highlight the `not` part of the does not match in unit test

6. Fix left sidebar options after updating library entry

7. Fix error handling when using `\C`

8. Fix debugger not handling empty data results

9. Made `\E` not quantifiable

10. Fixed some unicode property names for Java

11. Fixed unit tests sometimes not running when they should due to race condition

12. Remove truncating alternator check [https://github.com/firasdib/Regex101/issues/1556](https://github.com/firasdib/Regex101/issues/1556)

## 5.7.1 - 24th of March, 2021

1. Disallow backreferences inside character classes in Java

2. Fix binary unicode properties in Java

## 5.7.0 - 23rd of March, 2021

1. Fix explanation of character class intersection for Java

2. Fix regression in paste behavior [https://github.com/firasdib/Regex101/issues/1536](https://github.com/firasdib/Regex101/issues/1536)

3. Hardened verification for relative subpattern references

## 5.6.2 - 22nd of March, 2021

1. Fixed issue with `?` shortcut on certain devices [https://github.com/firasdib/Regex101/issues/1529#issuecomment-797851128](https://github.com/firasdib/Regex101/issues/1529)

2. Fixed regression in lookbehind quantifier validation for the PCRE flavor

3. Removed `\n` from substitutiton tokens in the quick reference for PCRE2

4. Hardened Java named backreference checker

5. Updated text displayed when browser is deemed too old to explain what is missing.

## 5.6.1 - 18th of March, 2021

1. Fix flags not explained when declared in group construct

2. Fix animation of left sidebar

3. Fixed link in match error section after engine fails to load

4. Fixed resize observer spamming error logs in quiz page

## 5.6.0 - 16th of March, 2021

1. Improved error handling

2. Disabled the use of `\k` in character classes in JS to avoid errors in certain browsers

3. Fixed issue when voting on certain library entries

4. Fixed Unicode escapes `\uNNNN` in java, accidentally accepted `\u{NNNN}` syntax

5. Disabled the use of quoted literals without any content as that has some ambiguous behavior

6. Fixes explanation regression [https://github.com/firasdib/Regex101/issues/1531](https://github.com/firasdib/Regex101/issues/1531)

## 5.5.3 - 15th of March, 2021

1. Fix regression in Javascript unicode parsing [https://github.com/firasdib/Regex101/issues/1530](https://github.com/firasdib/Regex101/issues/1530)

2. Add variable width lookbehind support to Java.
   The quantifiers `*` and `+` are disabled due to dodgy support in Java 8.
   In later versions (13+), the full regex syntax is supported (including backreferences).
   For now, neither backreferences nor the mentioned quantifiers will function in Java 8 on regex101

3. Fixed regression where `[^]` wasn't colored in JS mode

4. Fixed bug where unit tests were not ran if the regex switched from an error state to a non-error state

5. Disabled spell check for certain inputs where it was unnecessary/intrusive

6. Added clear indicator whether any test failed in the unit test view

7. Fixed subpattern parsing in subst mode for PCRE2

8. Fixed edge case when parsing java character classes that could result in `]` being treated literally

9. Fixed replacement in Java no handling trailing backslash properly

## 5.5.2 - 14th of March, 2021

1. Remove Disqus from library comments due to obscene ads

2. Handle stack overflow errors in Java

## 5.5.1 - 13th of March, 2021

1. Fixed parsing of `\R` in Java

2. Fixed parsing of named groups in Java

3. Updated some quickref entries

4. Fixed parsing of `\c` in PCRE2

5. Fixed parsing of whitespace while using the `x` flag in Java

## 5.5.0 - 12th of March, 2021

1. Made descriptions mandatory for library entries

2. Fixed library page not showing vote state on initial load

3. Added vote buttons to library details page to make voting easier

## 5.4.0 - 10th of March, 2021

1. Fixed issue where zero width match could erase the color of a same match at the same position

2. Added support for Java

3. Improved explanations for substitution tokens

4. Improved performance of the explanation engine

5. Increased contrast of white space visualization

6. Added link to regular-expressions.info when expressions time out

7. Fixed the PCRE2 substitution parser not catching all invalid escape sequences

## 5.3.1 - 6th of March, 2021

1. Fix issue with group painting when `\K` was used

2. Reduce size of export match button; makes it less obtrusive in the UI

3. Fix match info table on smaller screens

4. Fix monospaced font not applied properly in test area tooltips

5. Fixed explanation for `\b` being double escaped

## 5.3.0 - 5th of March, 2021

1. Updated the token colors for both themes. They are now easier on the eyes and aligned between the two.

2. Adjusted size of tooltips in editor

3. Adjusted the wording of tooltips when hovering regex tokens in the editor

4. Adjusted how \Q...\E is parsed and visualized in the editor.

5. Reworked the match information panel and made the space usage a bit more efficient. Reduced the amount of coloring in that region as well.

6. Updated styling of explanation area with regards to which items are highlighted and how.
   The goal is to reduce eye strain and color overload, and only color things that matter.

7. Adjusted wording in some of the explained entries.

8. Updated some entries in the quickref related to PCRE2 modifiers

9. Increased size of match export modal

10. Fix menus not easily closable on mobile

11. Fixed issue with library refetching entries unnecessarily

12. Added opengraph meta tags to index.html

13. Switched to source code pro as it seems to render better

14. Increased stroke contrast when hovering a match

## 5.2.8 - 25th of February, 2021

1. Adjusted how loading is done for sub-pages (no more blurring)

2. Quiz now makes a reduced amount of API calls for a better user experience

3. Fixed vote buttons on library page being incorrectly focusable

4. Improved contrast on library page

5. Increase size of quiz statistics chart

## Version 5.2.7 - 23rd of February, 2021

1. Updated relevance sorting algorithm for library page

2. Fixed bug where searches would randomly stop working on library page

3. Fixed race condition in list substitution mode for js flavor

4. Library entries now show their title in the header of the modal instead

5. Made the group numbers in the match info area focusable using tab

6. Added link to the debugger when catastrophic backtracking is detected

7. Automatically focus the input field in library view

8. Added button to easily navigate to library entry from regex editor

9. Improved load times of the website and placed theme code earlier in execution pipeline to avoid incorrect theme flashing

10. Fixed explanation of `\S` and `\W` in unicode mode.

11. Automatically set document title for the different parts of the website

12. Avoid transition flicker when loading pages on a fast connection

13. Add clear button to certain inputs

14. Update server configuration for better performance all around

15. Fix bug where small screens would not properly resize the substitution area

16. Fix issue where canvas would not repaint after closing the substitution area

## Version 5.2.5 - 21st of February, 2021

1. Reduced initial bundle size by code splitting more components that are not immediately necessary

2. Fixed focus outline of treeview arrows

3. Removed react-dom-server dependency (upstream react bug has since been fixed), further reducing bundle size

4. Improved accessibility of buttons by adding disabled attribute where applicable

5. Fixed surrogate validation for octal escapes

6. Switched to new service worker plugin, hopefully this works better!

7. Fixed multiple obscure issues reported by sentry, making the app more stable.

8. Added indicators to unit tests, alleviates some of the trouble color blind people might have with the new design. See [https://github.com/firasdib/Regex101/issues/1514](https://github.com/firasdib/Regex101/issues/1514)

## Version 5.2.0 - 16th of February, 2021

1. Added list substitution feature [https://github.com/firasdib/Regex101/issues/1410](https://github.com/firasdib/Regex101/issues/1410)

2. Increased font sizes throughout the app

3. Improved contrast ratio for dark theme

4. Fixed light theme flashing when loading website and dark theme was previously selected

5. Improved tooltip for conditionals [https://github.com/firasdib/Regex101/issues/1503](https://github.com/firasdib/Regex101/issues/1503)

6. Signing in will now save the state of the regex editor and restore it upon returning to the website.

7. Revamped unit test area [https://github.com/firasdib/Regex101/issues/1090](https://github.com/firasdib/Regex101/issues/1090)

8. Added new shortcuts. Hit `?` when not inside an editor. [https://github.com/firasdib/Regex101/issues/1088](https://github.com/firasdib/Regex101/issues/1088)

9. Improve text selection color

10. Increased the regex debugger domain to [0, 200] by default, instead of [0, 50]

11. Fix substitution area running match on mount with invalid substitution string

12. Fixed regex parser regressions

13. Switched monospace font to roboto mono

## Version 5.1.8 - 11th of February, 2021

1. Updated the display of the quiz statistics

2. Added method to revalidate quiz entries when the tests change

3. Fixed explanation for the `A` flag for PCRE/PCRE2 [https://github.com/firasdib/Regex101/issues/1498](https://github.com/firasdib/Regex101/issues/1498)

4. Fixed an issue where codemirror would cause a layout shift when initially rendered

5. Made JS `y` flag and PCRE `A` flag interchange when switching flavors [https://github.com/firasdib/Regex101/issues/1499](https://github.com/firasdib/Regex101/issues/1499)

6. Fix issue where the toolbar for the unit tests was shrunk down

7. Automatically switch to the unit test pane if there is no test/substitution string [https://github.com/firasdib/Regex101/issues/1502](https://github.com/firasdib/Regex101/issues/1502)

## Version 5.1.2 - 8th of February, 2021

1. Fixed regression in match highlighter [https://github.com/firasdib/Regex101/issues/1495](https://github.com/firasdib/Regex101/issues/1495)

2. Fixed issue where save modal would not highlight the value

3. Fixed issue where copy buttons would stop working

## Version 5.1.0 - 8th of February, 2021

1. Add code splitting

   - Split out large dependencies
   - Conditionally load polyfills
   - Lazy load certain components

   This might result in a few more quirks and bugs, but they will be ironed out with time.
   Please report any findings on [github](https://github.com/firasdib/Regex101/issues)

2. Remove large (unnecessary) dependencies

   Bundle size for initial load has been shrunk by around 30% with the above change.

3. Update PCRE2 to solve issue of number parsing (PHP and other implementers will have to do the same eventually)

4. Full rewrite of many components to improve accessibility

   - Tabbing is context aware
   - Navigation of entire site through tab
   - Aria tags added (not exhaustive, will be ongoing work)

   Hopefully this improves the experience for everyone!

5. Fixed issue where test area would not accurately highlight all strings

6. Fixed an issue where the markdown editors toolbar did not work as intended

7. Fixes links in quickref [https://github.com/firasdib/Regex101/issues/1489](https://github.com/firasdib/Regex101/issues/1489)

8. Removes duplicate entry in quickref [https://github.com/firasdib/Regex101/issues/1493](https://github.com/firasdib/Regex101/issues/1493)

9. Fixed issue where closing substitution area did not properly update the match coloring

10. Adds preloading to fonts and web worker

## Version 5.0.21 - 3rd of February, 2021

1. Fixed infinite loop when loading the page and subst box was open

2. Improve screen readers and SEO

## Version 5.0.19 - 2nd of February, 2021

1. Fix substitution area not triggering initially when opened

2. Fix subst indicator clipping

3. Fix subst area sometimes using invalid regex when performing subst (using cache is great...)

4. Fix issue where test input would not reset focus state

## Version 5.0.16 - 31st of January, 2021

1. Fixed backend not allowing users to unfavorite permalinks

2. Added ability to edit permalink details if signed in for favorited expressions through the save modal

3. Adjusted color for the resize strip in the right sidebar

4. Fixes validation of (?P>...) in PCRE

5. Added check to ensure null bytes aren't included in the regex for PCRE

## Version 5.0.13 - 30th of January, 2021

1. Add check to ensure numbers following backslashes are not too large

2. Update the default flavor to PCRE2

3. Explain `\s` and `\S` for javascript using unicode tokens instead of literal text

4. Fix substitution not running if test string was empty

5. Add support for non atomic lookarounds

## Version 5.0.12 - 28th of January, 2021

1. Fixed issue where the same input pasted into the regex input would not highlight syntax.

2. Treats `$$` as escaped literal in PCRE2 subst string

3. Fixed regression in `{m,n}` quantifier validation

4. Fixed invalid backref parsing for pcre2 (`\80` to `\99` was interpreted as ocals and literals)

5. Align the PCRE2 implementation with pcre2test wrt to empty matches at the end of the string

6. Fix text input focus issue [https://github.com/firasdib/Regex101/issues/1482](https://github.com/firasdib/Regex101/issues/1482)

7. Fix tags/titles not saved correctly

8. Show delete link in save modal for users who are not signed in

## Version 5.0.11 - 25th of January, 2021

1. Fixed bug in regex parser [https://github.com/firasdib/Regex101/issues/1477](https://github.com/firasdib/Regex101/issues/1477)

2. Added support for new PCRE2 features [https://github.com/firasdib/Regex101/issues/1476](https://github.com/firasdib/Regex101/issues/1476)

3. Updated tests for quiz task 27

4. Fix save modal not always selecting the generated url

## Version 5.0.10 - 24th of January, 2021

1. Patched numerous bugs that slipped through the initial release.

2. Updated quiz task 11 and 27 (Thanks David!)

3. Fixed issue with match timeout setting not working as intended

4. Increased memory limits for PCRE, PCRE2 and Python.

## Version 5.0.0 - 22th of January, 2021

1. Rewrote entire backend to improve performance

2. Reworked the account page; titles and tags are now associated with the entire
   permalink and not a specific version.

3. Redesigned the save modal, it now shows the account information (if signed in) in the same view,
   and makes it easier to work with.

4. Switched to new icons throughout the entire application

5. Slight modifications to the general look and feel, such as flatter buttons and larger font sizes.

6. Added support for PCRE2

7. Dropped support for legacy browsers, approximately the following versions: Internet Explorer, Firefox <55, Chrome <60, Edge <16

8. Reworked library entries: a permalink is now permanently associated with an account and the
   entry, and the owner can whenever they want update the version of that permalink which will reflect
   in the library. Hopefully this is not going to be abused, but if it is, the library will always
   default to the first version and never allow for an update.

9. Titles and tags are now associated with the entire permalink and all versions within it.

10. The default save functionality of the website has been changed, now a new permalink is created
    by default (using ctrl+s) and an update of the current workspace has to be explicit,
    by either clicking the menu item or using ctrl+shift+s.

11. The regex quiz now utilizes the PCRE2 engine instead of PCRE1.
    Can you exploit this to your advantage?

12. Multiple dependencies has been updated, which has resulted in a lot of behind-the-scenes work.
    This has resulted in general performance improvements, but nothing you are likely to experience.

13. Squashed 20-30 different edge case bugs in the app and regex tokenizer.
    I will outline fixes of this nature in the future, but for now, take my word for it.

14. The supported Python version is now indicated in the sidebar

15. Reorganized settings

16. Added a new setting that allows you to conditionally turn on/off step counting in supported
    flavors. This can dramatically improve performance in complex expressions.

17. Fixed key binding bug which would present itself in the debugger.

18. Added more tests to multiple quiz tasks.

19. Implemented surgical fix to avoid odd tabbing behavior in debugger (and other similar modals)

20. Added support for the # delimiter.

21. Due to 2 and 8, the database had to be modified, and data had to be migrated.
    Some loss of data is to be expected, since not all the information from the previous model could
    fit in the new one, but there are extremely few individuals affected.
    This only affects titles and tags, not any saved expressions.

22. Fixed autoit code generator

23. Fixed parsing and validation of surrogate pairs in the editor

24. Added a "whats new" button to the header

25. Revised contrast of dark theme

26. Increased font sizes slightly

27. Improved performance of tooltips in the editor (and possible squashed a few bugs that would cause the app to crash)

28. Rewrote large parts of the editor page (front page) and the regex parser. Hopefully I have not introduced (too many) new bugs...

29. Substitution area has received some love. A new indicator was added, similar to the match functionality.

30. Added PCRE2 native substitution (and the new syntax).

31. Fixed bug with `\b` in substitution
