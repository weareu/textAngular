<a name="1.5.18"></a>
## [1.5.18](https://github.com/fraywing/textAngular/compare/v1.5.17...v1.5.18) (2025-01-21)



<a name="1.5.17"></a>
## [1.5.17](https://github.com/fraywing/textAngular/compare/v1.5.16...v1.5.17) (2025-01-21)



<a name="1.5.16"></a>
## [1.5.16](https://github.com/fraywing/textAngular/compare/v1.5.15...v1.5.16) (2016-12-05)


### Bug Fixes

* **taFixChrome, taFixChrome.spec:** corrected a bug introduced when correcting pasted html (see PR [#1411](https://github.com/fraywing/textAngular/issues/1411)) ([35be0a0](https://github.com/fraywing/textAngular/commit/35be0a0))



<a name="1.5.15"></a>
## [1.5.15](https://github.com/fraywing/textAngular/compare/v1.5.14...v1.5.15) (2016-12-04)


### Bug Fixes

* **taBind:** (from damien-otis) Add code to handle pasting text in IE [#1410](https://github.com/fraywing/textAngular/issues/1410) ([b9863c2](https://github.com/fraywing/textAngular/commit/b9863c2))
* **taBind:** corrected bug [#1379](https://github.com/fraywing/textAngular/issues/1379) where the paste from word was broken for lists ([c11765d](https://github.com/fraywing/textAngular/commit/c11765d))
* **taFixChrome, taFixChrom.spec:** fixed bug where the html was being damaged on pasted html ([425396d](https://github.com/fraywing/textAngular/commit/425396d))
* Note: with this release we shift from tab's in the source code to 4 spaces!


<a name="1.5.14"></a>
## [1.5.14](https://github.com/fraywing/textAngular/compare/v1.5.13...v1.5.14) (2016-11-30)


### Bug Fixes

* **DOM:** corrected a bug where we could not insertHTML when the document was empty. ([ba156c4](https://github.com/fraywing/textAngular/commit/ba156c4))
* **taBind:** corrected a bug where we attempted to restore the selection in element.on('input') when the
     document was empty after a delete.
* **textAngularSetup):** corrected a bug where we would throw an error in taRegisterTool('justifyFull'),
     taRegisterTool('justifyRight'), and taRegisterTool('justifyLeft') when it was illegal to call
     .css('text-align).  We now catch and suppress those errors.


<a name="1.5.13"></a>
## [1.5.13](https://github.com/fraywing/textAngular/compare/v1.5.12...v1.5.13) (2016-11-10)


### Bug Fixes

* **main:** Corrected issue [#1353](https://github.com/fraywing/textAngular/issues/1353) where the dropEvent.target was not being used. ([be038c2](https://github.com/fraywing/textAngular/commit/be038c2))
* **main:** Corrected issue [#1359](https://github.com/fraywing/textAngular/issues/1359) and some older issues around refesh of popover display ([4ef827e](https://github.com/fraywing/textAngular/commit/4ef827e))
* **taBind:** Corrected issue [#1361](https://github.com/fraywing/textAngular/issues/1361) can't paste word document with tables ([f27d444](https://github.com/fraywing/textAngular/commit/f27d444))
* **taBind:** Corrected issue where Apple ignores Shift+Enter on Safari ([cd9de24](https://github.com/fraywing/textAngular/commit/cd9de24))
* **taBind, textAngular-sanitize:** Corrected and enhanced formating comming from Word and OneNote ([fbcd381](https://github.com/fraywing/textAngular/commit/fbcd381))
* **main:** Cleanup event handlers that are placed on the window (from Bret Little)
* **textAngularSetup:** Fix clear formatting functionality when used with ta-default-wrap=br #1374 - thanks to damien-otis for this fix. 0e45059062fadf2499b4d4d4f78621a49cb89968
* **taBind:** Fix don't deselect after 1000ms after applying styling #1381 - thanks to damien-otis for this fix 


<a name="1.5.12"></a>
## [1.5.12](https://github.com/fraywing/textAngular/compare/v1.5.11...v1.5.12) (2016-10-03)


### Bug Fixes

* **DOM:** Issue [#754](https://github.com/fraywing/textAngular/issues/754) is not corrected.  Now wrapSelection('insertHtml', embed, true) can insert '\n' ([424ac59](https://github.com/fraywing/textAngular/commit/424ac59))
* **main:** added a click monitor to the resize.background to shift the focus back to editor when closed. ([a3133ca](https://github.com/fraywing/textAngular/commit/a3133ca))
* **main:** Corrected issue editor only focuses when files are dropped - drop text behavior, Schamelhout
* **main:** Fix multi-deselect problem [#1334](https://github.com/fraywing/textAngular/issues/1334) from mikolawannabe ([64d0c4a](https://github.com/fraywing/textAngular/commit/64d0c4a))
* **taBind:** Corrected console errors caused by #text nodes - damien-otis. ([6dd1556](https://github.com/fraywing/textAngular/commit/6dd1556))
* **main:** Corrected issue [#299](https://github.com/fraywing/textAngular/issues/299) around the positioning of the popover on scrolling ([53f9529](https://github.com/fraywing/textAngular/commit/53f9529))
* **main:** Corrected Issue: [#1326](https://github.com/fraywing/textAngular/issues/1326) ([f9715de](https://github.com/fraywing/textAngular/commit/f9715de)) No reflowPopover() when window resized or scrolled. 
* **taBind:** Corrected 'MS Word, some word spaces get lost (line break issue?)' [#598](https://github.com/fraywing/textAngular/issues/598) ([e29e463](https://github.com/fraywing/textAngular/commit/e29e463))



<a name="1.5.11"></a>
## [1.5.11](https://github.com/fraywing/textAngular/compare/v1.5.10...v1.5.11) (2016-10-01)


### Bug Fixes

* **demo:** improved the style usage ([58f7f8d](https://github.com/fraywing/textAngular/commit/58f7f8d))
* **demo/textAngular.com.html:** fixed issue [#611](https://github.com/fraywing/textAngular/issues/611) by adding a 'clearfix' to the ta-text-editor-class attribute. ([3683747](https://github.com/fraywing/textAngular/commit/3683747))
* **DOM:** corrected bug [#1343](https://github.com/fraywing/textAngular/issues/1343) where we were incorrectly setting the <a> link on a <li> element ([44d5c56](https://github.com/fraywing/textAngular/commit/44d5c56))
* **factories:** small fix for undefined unsafe.replace [#1335](https://github.com/fraywing/textAngular/issues/1335) ([12a7b27](https://github.com/fraywing/textAngular/commit/12a7b27))



<a name="1.5.10"></a>
## [1.5.10](https://github.com/fraywing/textAngular/compare/v1.5.9...v1.5.10) (2016-09-19)


### Bug Fixes

* **DOM, globals, main, taBind:** Fix for [#1205](https://github.com/fraywing/textAngular/issues/1205) Duplicating content inside <p> ([581e050](https://github.com/fraywing/textAngular/commit/581e050))
* **DOM, taBind, taBind.spec:** added test for ShiftKey being pressed and released ([1b94314](https://github.com/fraywing/textAngular/commit/1b94314))
* **globals, taBind:** small code clean up and re-org ([19cfe7e](https://github.com/fraywing/textAngular/commit/19cfe7e))
* **main:** fix for [#655](https://github.com/fraywing/textAngular/issues/655) activeState seemingly not firing after the first click after a highlight [#655](https://github.com/fraywing/textAngular/issues/655) ([6ecc1c1](https://github.com/fraywing/textAngular/commit/6ecc1c1))
* **main:** fixed an invalid error in rare conditions ([8772907](https://github.com/fraywing/textAngular/commit/8772907))
* **taBind:** Browser spelling correction not setting the control to dirty [#1120](https://github.com/fraywing/textAngular/issues/1120) ([5473d01](https://github.com/fraywing/textAngular/commit/5473d01))
* **taBind:** corrected issue #607 - catching Ctrl+Return ([438e060](https://github.com/fraywing/textAngular/commit/438e060))
* **DOM, globals, main, taBind:** Fix for #1205 Duplicating content in ... (https://github.com/fraywing/textAngular/commit/581e050a3ed5bb4f21d59e4a59856f1d4a859770)


<a name="1.5.9"></a>
## [1.5.9](https://github.com/fraywing/textAngular/compare/v1.5.8...v1.5.9) (2016-09-05)


### Bug Fixes

* **factories.js:** removed the extra <span id="selectionBoundary..." class="rangySelectionBoundary">></span> and ([76a31e2](https://github.com/fraywing/textAngular/commit/76a31e2))
* **main:** We now properly update the toolbar when we tab into the editor. ([d930538](https://github.com/fraywing/textAngular/commit/d930538))
* **DOM, textAngularSetup, taExecCommand.formatBlock.spec, taTools.spec)
 - removed a rare element.parentNode === null condition
 - fixed a rare bug during 'CLEAR' formatic where we could see a rangy error
   'The given range isn't in document'
 - enhanced the 'CLEAR' format function to properly handle nested <ul> statements

#### Features
  * Enhancment: - the build proces is improved and we are now uptodate with the
                packages in use.  Only grunt-istanbul-coverage is behind because
                it currently breaks the  build.
              - Updated the grunt-conventional-changelog to the current package.
                and added an editing step for the changelog.md as part of the
                build process.

#### Breaking Changes (BUILD ONLY)
  * Because of the update of the packages used in the build process, you must
    do a 'npm install' before you can build.



<a name"1.5.8"></a>
### 1.5.8 (2016-08-31)


#### Bug Fixes

* **textAngular:**
   * Fixed several issues around Italic, Bold, Strikethrough, Underline state in the  ([7823937b](https://github.com/fraywing/textAngular/commit/7823937b))
   * fix(DOM, textAngularSetup): Functionality under Firefox is now much improved. 
   * Build Enhancement: updated many of the development packages.  There is more work to do, but some improvement.
   * Fix(main): removed the saveFocusSelection() and restoreFocusSelection()
      which to do function properly and create problems!

#### Features
   * Enhancment: - 'insertLink' now allows editing of existing link


<a name"1.5.7"></a>
### 1.5.7 (2016-08-23)


<a name"1.5.6"></a>
### 1.5.6 (2016-08-23)


#### Bug Fixes

* **textAngular:**
  * Fix(main, textAngularManager.spec): Corrected issues with toolbar being active all all editors with same toolbar.
     Now toolbarScopes are tied to each editor which is cleaner and makes more sense.
      AND the toolbarScopes are deleted when the editor is deleted which is better and
      no longer tied to the toolbar.
      We also added some code to enable $log messages in the karma testing when necessary
      See the textAngularManager.spec.js file for details looking at 'var $log', beforeEach() and afterEach()
     (https://github.com/fraywing/textAngular/commit/daec3e8769f187be3e9f9f5a3c4ac33241f3e492) 
  * Fix(taFixChrome.spec): added a test to verify the fix form #1281 (https://github.com/fraywing/textAngular/commit/cd45b29a9fddeffaab5bae267572a59b04bd0370)
  * Fix(main): We now respect he selection and enhanced wrapSelection (https://github.com/fraywing/textAngular/commit/13379176e7b732bf8b83aee9fe0fa5104dcf3473)
  * FIx(Gruntfile): Added the missing task demo_pages to all release paths
  * Chore(README): Update to new pluker link
      
* **factories:**
  * Only append remainder if the Apple-converted-space has matched ([e086974c](https://github.com/fraywing/textAngular/commit/e086974c))
  * Add remainder of html string to finalHtml ([950ed2d8](https://github.com/fraywing/textAngular/commit/950ed2d8))



<a name"1.5.6-0"></a>
### 1.5.6-0 (2016-08-17)

* **textAngular:**
  * Enhancement(demo, static-demo, textAngular.com) Added version display to demo code 
           (https://github.com/fraywing/textAngular/commit/3c3ce76c3805d67e49c980c5bf1da15f52a24781)
  * Enhancement(main, globals, Gruntfile, textAngularManger.spec, textAngular.spec): 
       Added a new directive text-angular-version and a new function to textAngularManger:getVersion()
       I have wanted to add this for a long time to make it easier to display the version of textAngular being used.
           (https://github.com/fraywing/textAngular/commit/1ffa6f7263ce844a4e300226616a9d2282143f56)
       This also modifies the build process to automatically put the version into globals.js     

<a name"1.5.5"></a>
### 1.5.5 (2016-08-15)

* **textAnglar:**
  * Fix(DOM, globals, main, taBind, textAngular.spec): Resoved the issues around the improvements from v1.5.4
       The bulk of the changes can be seen here: https://github.com/fraywing/textAngular/commit/c39f20d9cf2372f94b579d018b0cb9bb553e33ef
       
       
<a name"1.5.4"></a>
### 1.5.4 (2016-08-06)

* **textAnglar:**
  * Fix(DOM, globals, textAngular.spec): Corrected bugs around Firefox weirdness  (https://github.com/fraywing/textAngular/commit/32aad73a258696ae06d2ee6cc901bd571d7793fb)
         - DOM: major fix to handle Firefox weirdness around <br> insertions
                We now insert zero width spaces in place of <br> that is
                a '&#8203' character.
                This corrects taExecCommand() to function properly on Firefox.
         - globals: stripHtmlToText() now handles zero width spaces
         - textAngular.spec: added test for zero width spaces
  *  Enhancement(added Support for font-style = italic and font-size = [size em/px/%] in sanitize function validStyles,  (https://github.com/fraywing/textAngular/commit/dde3d7f621c7d4403577853374223abe5c9d15db)
                 Merge pull request #964 from rdkleine/master
  *  Fix(main, taBind, textAngularSetup, globals, taTools.spec): Immproved the issues 
          with html and model getting out of sync (https://github.com/fraywing/textAngular/commit/5453c6b8fd2d72c6bdfb1dd83cb9fc0ed6df0a88)
          Also corrected issue under Firefox where the initial selection was before all the content
          - globals: improved stripHtmlToText() slightly
          - main: fixed a mistyped if in switchView()
          - taBind: small formatting changes for clarity
                    improved element.on('keyup') code
                    element.on('focus') now detets an bad selection condition under Firefox and fixes this
          - textAngularSetup: added a coverage comment in recursiveRemoveClass() that is now needed
            because of changes to taTools.spec
          - taTools.spec: Changed the test set 'test clear button' so that now the whole
                          htmlcontent is now never selected.  This was an issue beacuse when
                          all the htmlcontent was selected this triggered the element.on('focus') fix
                          for Firefox and broke the tests here.  All the tests now run properly.
                          The biggest change was to now wrap the test content in a <div class='test-class'></div>
                          which caused the expected values to change.
  *  Fix(main, globals): Corrected issue with clobering the html from the model too easily. (https://github.com/fraywing/textAngular/commit/b1206a892bc104cb63a74633395d00c0d6ee39ed)
                          Added getDomFromHtml() and corrected when this is used.
  *  Fix(main): Corrected issues with html and model getting out of synch! (https://github.com/fraywing/textAngular/commit/91fe5bfb7fd17d345f2cdaace9c3f891a6ce2fbc)
  *  Fix(taBind, textAngular.spec): Major change to _taBlankTest() that now uses the DOM to check the visibility of the html
                     This removes the MANY headaches of the old code... that that very fragile.
         - added a new tool to measure performace where needed
         - added a global stripHtmlToText() function
         - added a new test to verify the performance tool and new stripHtmlToText() function
         (https://github.com/fraywing/textAngular/commit/31cf9c4d307a02aa9f078daceea9bd38a7d70c3a)
                               
                               
<a name"1.5.3"></a>
### 1.5.3 (2016-07-29)

#### Bug Fixes

* **textAngular:**
  * Fix(textAngularManager): Corrected bug #1231 Leaking memory scopes (https://github.com/fraywing/textAngular/commit/a0024a24a3ca0c40a3cd0ffed0edbc475f2a91ff)
  * Feat(textAngularManager): Added a function updateStyles() to force all the updateSelectedStyles() to be updated.  
                              This also now automatically sets up the initialization for tools in most cases. (https://github.com/fraywing/textAngular/commit/d373fe10e770bf521641975cbc6a4f480d0a1f9e)
  * Fix(main): Very small tweak in setupTriggerUpdateStyles() to accept the default $interval call that invokes a 
               $apply which will be more robust. (https://github.com/fraywing/textAngular/commit/0d860d0a97c440b868639bfb3ea9f3f943658da6)
  * Enhancement(main): Show switch HTML button all the time. Originally from ershwetabansal (https://github.com/fraywing/textAngular/commit/db1f5a0bb50019c56ff8863c8a42fdbef2ce53ab)                                           
  * Fix(textAngularSetup): We now block javascript for 'insertLink', 'insertVideo', and 'insertImage' issue: #1189 (https://github.com/fraywing/textAngular/commit/37e3f7acdb7099d825480b45cb55da7c756a0ae7)
  * Fix(taBind): corrected issue around Model becomes empty after edit Issue: #1230 (https://github.com/fraywing/textAngular/commit/17b4497ec3bd3939571724e4c9aad145d51e776c)                           


<a name"1.5.2"></a>
### 1.5.2 (2016-07-15)

#### Bug Fixes

* **textAngular:**
  * Fix(textAngularSetup): Corrected bug #1201 due to an issue with Firefox. (https://github.com/fraywing/textAngular/commit/dab42a371f03a6912de9b6310db5911b52cd8362)
  * docs(README): fix textAngular-santize.min.js typo (https://github.com/fraywing/textAngular/commit/12580ad5585611257c5a0888186fe24e57c4d862)
  * docs(README): update links to cdnjs and jsdelivr (https://github.com/fraywing/textAngular/commit/0ef205254360790ed45ab225171cc448d4730515)
  * Fix(DOM): merged fix from Hike-zzz: fixing issue #616 #1174 (https://github.com/fraywing/textAngular/commit/328cd69c06c5d13c2c7a9c4cfeb9406334295137)
  * Fix(README): fix typos- pull request #1072 from pra85/patch-2 (https://github.com/fraywing/textAngular/commit/0f7f2e4ce9c4a12a5c20c8f930fc8cee38d9287b)
  * Fix(taBind): fix for bug under Firefox when delete all content #1217 (https://github.com/fraywing/textAngular/commit/67e7ebe1003f439fa6a93c0f70cbb1818926522b)
  * Fix(textAngularSetup): bug #1223 InsertImage tool failed on Firefox (https://github.com/fraywing/textAngular/commit/f5e9bd4c5de55979572075cf4934b50201eb7a3e)
  * Fix(globals, taBind): browser previos fix no more needed (https://github.com/fraywing/textAngular/commit/8cd3e5a64a798adfda17fb1e9a3a91930f96e5e2)

#### Features

* **textAngular** Enhanced (factories): to do Better removal of style junk which Chome inserts. Also one bug fix in the old existing code (a missing /"). (https://github.com/fraywing/textAngular/commit/7d5d37cfa03cc75e012885920ea4939460020658)

<a name"1.5.1"></a>
### 1.5.1 (2016-04-25)


<a name"1.5.0"></a>
## 1.5.0 (2016-01-16)


#### Bug Fixes

* **main.js:**
  * we now hide the popover at the end of the image resize. ([c182c96c](https://github.com/fraywing/textAngular/commit/c182c96c))
  * we now hide the popover at the end of the image resize. ([d9cfcf15](https://github.com/fraywing/textAngular/commit/d9cfcf15))
  * Fix for #862 where the model was not changing after image resize. ([d5a508e3](https://github.com/fraywing/textAngular/commit/d5a508e3))
* **taBind.js:** Fix bug #843 -- improper closing of list elements ([a0b79276](https://github.com/fraywing/textAngular/commit/a0b79276))
* **textAngular-santitize:** Fix for internal model ignores style attr #854 ([9fc7288b](https://github.com/fraywing/textAngular/commit/9fc7288b))


<a name"1.4.6"></a>
### 1.4.6 (2015-09-20)


#### Bug Fixes

* **textAngular:**
  * Fix(textAngular): several bug fixes related to pasting from word. Closes #644, #617 ([f7d34a33](https://github.com/fraywing/textAngular/commit/f7d34a33658d7f336c2891cf9618ba34956c5bad))  
  * Fix(textAngular): several bug fixes related to pasting from word. Closes #644, #617 ([f7d34a33](https://github.com/fraywing/textAngular/commit/f7d34a33658d7f336c2891cf9618ba34956c5bad))  
  * Fix(npm): bad package for 1.4.5 is updated to current version. Closes #888

#### Features

* **textAngular:** textAngular-sanitize now respects and keeps most whitespace and html comments! ([aba8265](http://github.com/fraywing/textAngular/commit/aba826510f5356318673c622cfa55be512801581), closes [#846, #847]
* **textAngularSetup:** textAngularSetup - fixed dependency issue with textAngularSetup to all use of constant taRegisterTool. Closes PR #866 (https://github.com/fraywing/textAngular/pull/866)


<a name"1.4.5"></a>
### 1.4.5 (2015-09-15)
 * Fix(css): fixed css/js mistake in the 1.4.4 release!

<a name"1.4.4"></a>
### 1.4.4 (2015-09-12)


#### Bug Fixes

* **coverage:** Gruntfile -- coverage back to 100% and fixed the banner. ([55f2c9a3](https://github.com/fraywing/textAngular/commit/55f2c9a3))
* **gitcommit:** Demo pages was not being included ([aa570e87](https://github.com/fraywing/textAngular/commit/aa570e87))
* **textAngular:**
  * Fix(main): tests weren't running without requireJS ([e40874ad](https://github.com/fraywing/textAngular/commit/e40874ad)
  * Fix issue with two baners being included in the build ([776db53](https://github.com/fraywing/textAngular/commit/776db53))
  * Fix memory leak for event window.blur ([bd3e84f1](https://github.com/fraywing/textAngular/commit/bd3e84f1))
  * Fix 644 parse whitespace from plaintext ([5c028f5b](https://github.com/fraywing/textAngular/commit/5c028f5b))
  * Fix(Readme): Plunkr was not loading ([e10644de](https://github.com/fraywing/textAngular/commit/e10644de2))
  * Fix image resize ([e9d6f079](https://github.com/fraywing/textAngular/commit/e9d6f079))
  * fix popover requires 2 clicks to hide ([fed6cca0](https://github.com/fraywing/textAngular/commit/fed6cca0))


#### Features

* **textAngular:** Full support for commonjs (Closes #737, #712, #713, #716, #708, #709, #853) ([a0a84553](https://github.com/fraywing/textAngular/commit/a0a84553))
* **demo:** Updated the demo pages to 1.4.3 ([ddd000df](https://github.com/fraywing/textAngular/commit/ddd000df))


<a name"1.4.3"></a>
### 1.4.3 (2015-07-30)


#### Bug Fixes

* **textAngular:** Fix image resize broken for chrome ([86072d4b](https://github.com/fraywing/textAngular/commit/86072d4b))
* **textAngularSetup:** Inorder to fully block Undo or Redo, one must also call event.preventDefault() ([aedc38e4](https://github.com/fraywing/textAngular/commit/aedc38e4))
* **textAngular:** Fix remove CSSRule-when-no-rules ([0eb2f38](https://github.com/fraywing/textAngular/commit/86072d4b))

#### Features

* **taToolbar:** Update insertVideo to handle youtube link variants ([1372bc1d](https://github.com/fraywing/textAngular/commit/1372bc1d))
* **test:** Added coverage for 'justifyFull' button. ([72cca334](https://github.com/fraywing/textAngular/commit/72cca334))
* **textAngularSetup:**
  * Added taOptions.keyMappings to customize key bindings. ([05546ab4](https://github.com/fraywing/textAngular/commit/05546ab4))
  * Added taOptions.keyMappings to adjustment the key bindings for Redo, Undo, ... ([de12e3e3](https://github.com/fraywing/textAngular/commit/de12e3e3))
  * Added a taOptions:forceTextAngularSanitize to verify sanitizer provider. ([ad04836b](https://github.com/fraywing/textAngular/commit/ad04836b))
  * Added a taOptions:forceTextAngularSanitize to verify sanitizer provider. ([8e642c15](https://github.com/fraywing/textAngular/commit/8e642c15))

#### Breaking Changes

If you were using a different sanitize provider instead of textAngular-sanitize we will now detect this and throw an error.  To eliminate this error set taOptions.forceTextAngularSanitize: false

<a name"1.4.2"></a>
### 1.4.2 (2015-07-15)

#### Bug Fixes

* **textAngular:** corrected undefined event #796 ([6186ed52](https://github.com/fraywing/textAngular/commit/6186ed52))
* **taBind:** Reapply selector handles on focus ([f05857e3](https://github.com/fraywing/textAngular/commit/f05857e3))
* **textAngular:** Fixed resize image issue ([52fb20c0](https://github.com/fraywing/textAngular/commit/52fb20c0))
* **grunt:** Update javascript path in watch target ([58df955d](https://github.com/fraywing/textAngular/commit/58df955d))
* **textAngular:**
  * Fixed test coverage when commonElement is document ([b807423b](https://github.com/fraywing/textAngular/commit/b807423b ))
  * Fixed corner case when commonElement is document ([dbea6244](https://github.com/fraywing/textAngular/commit/dbea6244))
  * Use CSS instead of html attributes to resize image. ([a84f6df4](https://github.com/fraywing/textAngular/commit/a84f6df4))
  * Fix resize image issue ([52fb20c0](https://github.com/fraywing/textAngular/commit/52fb20c0))

#### Features

* **textAngular:** 
   * Added directives ta-resize-keep-aspect-ratio and ta-resize-maintain-aspect-ratio to control image-resize ([32697058](https://github.com/fraywing/textAngular/commit/32697058))
   * Added input to the safe element list ([945cfa00](https://github.com/fraywing/textAngular/commit/945cfa00))
* **textAngularDemo:** Updated the demo to be in synch with this release ([93fd4048](https://github.com/fraywing/textAngular/commit/93fd4048))
* **globals:** Added aria-hidden to hidden input, to hide it from screen readers ([b49bf814](https://github.com/fraywing/textAngular/commit/b49bf814))
* **textAngularSetup:** Enhanced toolbar to handle TAB and SHIFT-TAB KEYS. ([8df51fb](https://github.com/fraywing/textAngular/commit/8df51fb))
* **taToolFunctions:** Create factory for sharable functions ([032611dd](https://github.com/fraywing/textAngular/commit/032611dd))

<a name="1.4.1"></a>
### 1.4.1 (2015-05-25)

#### Breaking Changes

This changes the structure of the files - all production files are now in the dist folder, this makes where PR's should be done a little more clear.

If you were referencing the src/*.js files they will need to be updated to dist/*js.

#### Bug Fixes

* **taPaste:** Fix the taPaste order s.t. sanitizer is called after paste handler. ([108857f6](http://github.com/fraywing/textAngular/commit/108857f69ac611f970ded65ba5c1207b8a6964d0), closes [#686](http://github.com/fraywing/textAngular/issues/686))


<a name="1.4.0"></a>
## 1.4.0 (2015-05-24)

#### Breaking Changes

The minimum required versions of AngularJS is 1.3 and Rangy is 1.3.

#### Bug Fixes

* **chrome:** Make the matcher for detecting bad chorem tags more lenient ([05fe7a61](http://github.com/fraywing/textAngular/commit/05fe7a61470d41b6533f5220894ec1a3451dc801))
* **taBind:** Updating while focussed. ([cc6d89be](http://github.com/fraywing/textAngular/commit/cc6d89bee18de5a2666aae075c707ae7aa68cb9f), closes [#38](http://github.com/fraywing/textAngular/issues/38))
* **taBind.formatters:** Catch unwrapped content ([0cd98dd3](http://github.com/fraywing/textAngular/commit/0cd98dd3115f4e7d09263eeeb0136ec9d2ccaafa), closes [#584](http://github.com/fraywing/textAngular/issues/584))
* **taBind.keyevents:** Attempted fix for polish character issues ([26226dda](http://github.com/fraywing/textAngular/commit/26226ddaa9f5468977f3a4849e265904ca2fad6a), closes [#518](http://github.com/fraywing/textAngular/issues/518))
* **taBinde.undomanager:** Fix a bug with redo/undo beyond the borders ([dd023c30](http://github.com/fraywing/textAngular/commit/dd023c30537cd79550de630f7d4360331eb02975), closes [#558](http://github.com/fraywing/textAngular/issues/558))


* **taTools:** Added options for tools in taOptions ([7fb00a02](http://github.com/fraywing/textAngular/commit/7fb00a02993f8c02b09f8a24c3c267b6ba4f8fbd))


<a name="1.3.11"></a>
### 1.3.11 (2015-03-16)


<a name="1.3.10"></a>
### 1.3.10 (2015-03-16)


#### Bug Fixes

* **placeholder:** multiple textAngular will cause CSSRule index error ([943f08d5](http://github.com/fraywing/textAngular/commit/943f08d5b1ccc1c358071e67f5968267a0664299))


<a name="1.3.9"></a>
### 1.3.9 (2015-03-13)


#### Bug Fixes

* **taBind.$formatters:** Fix an issue where unwrapped tags broke the textarea display ([d39c7b63](http://github.com/fraywing/textAngular/commit/d39c7b63732b345b826068de4f9655d082d74262), closes [#566](http://github.com/fraywing/textAngular/issues/566))


<a name="1.3.8"></a>
### 1.3.8 (2015-03-13)


#### Bug Fixes

* **taBind:** Fix tab focus issue. ([8693e1d6](http://github.com/fraywing/textAngular/commit/8693e1d69daf44bb4ca6a94863bd2e43b598f571), closes [#483](http://github.com/fraywing/textAngular/issues/483), [#379](http://github.com/fraywing/textAngular/issues/379))
* **textAngular.popover:** Add scroll top offset. ([f12eb86d](http://github.com/fraywing/textAngular/commit/f12eb86d7dd473244f09982dc1b13b0e0949ca5c))


<a name="1.3.7"></a>
### 1.3.7 (2015-02-13)


#### Bug Fixes

* **taSanitize:** Close XSS vector, See http://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-0167, http://xforce.iss.net/xforce/xfdb/100929 and https://exchange.xforce.ibmcloud.com/#/vulnerabilities/100929 for details. ([f5f27c26](http://github.com/fraywing/textAngular/commit/f5f27c26bc99dc6f8bb226d7beb99ce8bcada01a))


<a name="1.3.6"></a>
### 1.3.6 (2015-02-06)


#### Bug Fixes

* **taSelection:** Fix selecting end of element being after trailing <br> ([e1008dfc](http://github.com/fraywing/textAngular/commit/e1008dfc02592b8484ff618bafbcd7f30084b8e4))


#### Features

* **taBind:** Allow updates while focussed. ([452c7f01](http://github.com/fraywing/textAngular/commit/452c7f010aea73a69d09672623b5deb6b8a32bf4), closes [#38](http://github.com/fraywing/textAngular/issues/38))


<a name="1.3.5"></a>
### 1.3.5 (2015-02-05)


#### Bug Fixes

* **globals:** Fix document.head undefined in IE<9 ([da435392](http://github.com/fraywing/textAngular/commit/da435392a099d2ce7aaf63458556fe64831426f6), closes [#530](http://github.com/fraywing/textAngular/issues/530))
* **sanitize:** Port script/style fix over from main repo. ([7975a26d](http://github.com/fraywing/textAngular/commit/7975a26d81b24c45c27af147ea86df6e12d2022d), closes [#533](http://github.com/fraywing/textAngular/issues/533))
* **taBind.paste:** Fix some paste isuses. ([f989f6c2](http://github.com/fraywing/textAngular/commit/f989f6c2fd4251d94f80387d00098fe4f31970f0))
* **taSelection:** Fix a bug in insert HTML. ([7003b27b](http://github.com/fraywing/textAngular/commit/7003b27bb110a5c7f0909e77f5c033fe35766fb0))


#### Features

* **ta-hidden-input:** Add new class for hidden inputs ([07eda5a8](http://github.com/fraywing/textAngular/commit/07eda5a8768c7171efc905d7b95f7fd5375d3c99))
* **ta-paste:** Add attribute that allows intercetping of the pasted content. ([39698985](http://github.com/fraywing/textAngular/commit/39698985dbc6a7a83be7328b3f89b42b0d948d39))
* **taDOM:** New services or dealing with html nodes ([a08bdc53](http://github.com/fraywing/textAngular/commit/a08bdc538b50f3cbc283877a90b380c6e77dacf1))


<a name="1.3.4"></a>
### 1.3.4 (2015-02-02)


#### Bug Fixes

* **dependancies:** Changed Bootstrap to Bootstrap-css-only ([9250bf5a](http://github.com/fraywing/textAngular/commit/9250bf5a32ea5a76be0c7fb605bb499df775b1b4), closes [#527](http://github.com/fraywing/textAngular/issues/527))
* **npm:** Fix installation issues with npm ([902fa692](http://github.com/fraywing/textAngular/commit/902fa692eed54211099af3e4e4a70eb060d46fe1), closes [#522](http://github.com/fraywing/textAngular/issues/522))


<a name="1.3.3"></a>
### 1.3.3 (2015-01-28)


#### Bug Fixes

* **taBind._blankTest:** Fix for highly nested content. ([4bbfbaba](http://github.com/fraywing/textAngular/commit/4bbfbabae7f85c810f1a614bb515a1454d3fb29c), closes [#512](http://github.com/fraywing/textAngular/issues/512))
* **textAngularSetup:**
  * Add tooltips for buttons on edit link popover ([0f980d3f](http://github.com/fraywing/textAngular/commit/0f980d3fc72959e42a3ba81e068fad5911454014))
  * Add translation for "Open in New Window" button on edit link popover ([d61ff1da](http://github.com/fraywing/textAngular/commit/d61ff1da442be64b647ba4341bc8099aea0e3967))


<a name="1.3.2"></a>
### 1.3.2 (2015-01-27)


#### Bug Fixes

* **dependancies:** Revert back to stable rangy version ([498176d2](http://github.com/fraywing/textAngular/commit/498176d21ee056ac5fd0348b9a6c8309ab27312e))
* **taSanitize:** Fix issue with last pre-tag overwriting all previous. ([230e779e](http://github.com/fraywing/textAngular/commit/230e779e9b9ae6f2de59a3e53e1def55420b8dd2), closes [#508](http://github.com/fraywing/textAngular/issues/508))


<a name="1.3.1"></a>
### 1.3.1 (2015-01-23)


#### Bug Fixes

* **Bower:** Rangy-official renamed to rangy. ([652204c9](http://github.com/fraywing/textAngular/commit/652204c9e2b271eee51159c27f90d1a429c0acb1))


<a name="1.3.1"></a>
## 1.3.1 (2015-01-23)


#### Bug Fixes

* **Bower:** Rangy-official renamed to rangy. ([652204c9](http://github.com/fraywing/textAngular/commit/652204c9e2b271eee51159c27f90d1a429c0acb1))


<a name="1.3.0"></a>
## 1.3.0 (2015-01-22)


#### Features

* **taBind:**
  * Textarea basic formatting of html with tabs and newlines ([f0d3baf8](http://github.com/fraywing/textAngular/commit/f0d3baf8dd99e11f746e6aa17ccf1e94c2842a87), closes [#307](http://github.com/fraywing/textAngular/issues/307))
  * Allow the events to be overriden in external directives ([c4b7bdda](http://github.com/fraywing/textAngular/commit/c4b7bdda609deb49d4c51cacd835c4082843c14b), closes [#493](http://github.com/fraywing/textAngular/issues/493))


<a name="1.3.0-23"></a>
### 1.3.0-23 (2015-01-20)


#### Bug Fixes

* **taBind:** Issue when unwrapped text was entered ([51f37284](http://github.com/fraywing/textAngular/commit/51f37284156bd2fca17a2c9aa7e42176393bf115), closes [#484](http://github.com/fraywing/textAngular/issues/484))


<a name="1.3.0-22"></a>
### 1.3.0-22 (2015-01-13)


#### Bug Fixes

* **main.events:** ng-focus wasn't being triggered on focus. ([3928bc50](http://github.com/fraywing/textAngular/commit/3928bc50205fb53de8c7cc08e213fc4f0b6aca24), closes [#482](http://github.com/fraywing/textAngular/issues/482))
* **taBind._blankTest:** Fix a bug where the first tag had really big attributes and cut off the actual c ([fe800b24](http://github.com/fraywing/textAngular/commit/fe800b24cbcfad53f2e9a0b793b1ead9b7b4d45e), closes [#484](http://github.com/fraywing/textAngular/issues/484))


<a name="1.3.0-21"></a>
### 1.3.0-21 (2015-01-06)


#### Bug Fixes

* **taBind:** Add blankTest tests and seperate service ([c3900a4a](http://github.com/fraywing/textAngular/commit/c3900a4a64c9b51632bc70c0e305d2752faa0ba3))
* **textAngular.resize:** Fixes resize overlay with more than one image ([c08ddd75](http://github.com/fraywing/textAngular/commit/c08ddd75282cea89e5c2bfed64bee7fc2f78b1a5), closes [#470](http://github.com/fraywing/textAngular/issues/470))


<a name="1.3.0-20"></a>
### 1.3.0-20 (2015-01-05)


#### Bug Fixes

* **textAngular.resize-overlay:** Catch when height or width is NaN ([efcb4115](http://github.com/fraywing/textAngular/commit/efcb411523aecab53a1798a7c25057f34f461444), closes [#470](http://github.com/fraywing/textAngular/issues/470))
* **textangular:** Fix focus issues in IE11 ([a5200e38](http://github.com/fraywing/textAngular/commit/a5200e38780744ad71aa30f83871917a22fd8471), closes [#443](http://github.com/fraywing/textAngular/issues/443))


<a name="1.3.0-19"></a>
### 1.3.0-19 (2014-12-18)


#### Bug Fixes

* **taBind:** Catch edge case on mouseup handler when no children ([e1140893](http://github.com/fraywing/textAngular/commit/e11408932653cb1e8adfae628fa34c495c7892bf), closes [#446](http://github.com/fraywing/textAngular/issues/446))
* **textAngular:** Add stop of update selected styles on blur. ([c877991d](http://github.com/fraywing/textAngular/commit/c877991de312b7e78865d4f03390de5a2e4d40c2), closes [#443](http://github.com/fraywing/textAngular/issues/443))


<a name="1.3.0-18"></a>
### 1.3.0-18 (2014-12-17)


#### Bug Fixes

* **textAngular:** Fixes the window blur check for updating styles ([72a5da81](http://github.com/fraywing/textAngular/commit/72a5da815ba8cad96ec70ab920dcf14971bdb05d))


<a name="1.3.0-17"></a>
### 1.3.0-17 (2014-12-16)


<a name="1.3.0-16"></a>
### 1.3.0-16 (2014-12-16)


#### Bug Fixes

* **taBind:**
  * Ensure onSelectHandlers are allways applied with DOM changes ([01873453](http://github.com/fraywing/textAngular/commit/0187345359cb833a43f76bd6385e67f79193c84c), closes [#446](http://github.com/fraywing/textAngular/issues/446))
  * Fix cursor selection on focus ([05f15a5e](http://github.com/fraywing/textAngular/commit/05f15a5e4adcd4d21cd3b9085bcd031e5d0e0c65), closes [#444](http://github.com/fraywing/textAngular/issues/444))
  * _blankTest should be more performant now and stop crashing chrome ([57ff7ba1](http://github.com/fraywing/textAngular/commit/57ff7ba1d6154ef9202fe13aacc4a3efe1da2d87), closes [#451](http://github.com/fraywing/textAngular/issues/451))
* **taBind.paste:** Fix multi-paste issue ([58f75379](http://github.com/fraywing/textAngular/commit/58f7537926368a1da96c614f0c02790029e1f284), closes [#392](http://github.com/fraywing/textAngular/issues/392))
* **taSanitize:**
  * Fix inconsistencies between browsers of bold, italics and underline ([dd479a16](http://github.com/fraywing/textAngular/commit/dd479a166a054fcd4f2defada0b72a0fc84777ea))
  * fix also container (#424) ([a49600de](http://github.com/fraywing/textAngular/commit/a49600de089281b5562cdad8d7ccefa7e905baf5))
  * add test (#424) ([2b94c7c1](http://github.com/fraywing/textAngular/commit/2b94c7c1dca4dde0aa3f9bfe534649f2a5070235))
  * copy code to lib/factories.js (#424) ([e61f69c0](http://github.com/fraywing/textAngular/commit/e61f69c075ec56a7499df9894b881f4ef634ed10))
  * merge taPreSatitize to taSanitize (#424) ([e3c9cf6e](http://github.com/fraywing/textAngular/commit/e3c9cf6e665b6e92fe5fc5d62ded35407e15743c))
  * fix for #424 ([91b16c89](http://github.com/fraywing/textAngular/commit/91b16c89fa2176d2bc27ec804f4d08fb5d471ccd))
* **textAngular:** Prevent updateSelectedStyles loop when out of document focus ([81a37de7](http://github.com/fraywing/textAngular/commit/81a37de7a48b1d17933843c07559398c0c430ad5))


<a name="1.3.0-pre15"></a>
### 1.3.0-pre15 (2014-12-05)


#### Bug Fixes

* **DOM:** Fix for convert to lists ([75cc1441](http://github.com/fraywing/textAngular/commit/75cc14418a7c8cde971b37847d2025a3f4c6abee), closes [#377](http://github.com/fraywing/textAngular/issues/377))
* **placeholder:** add missing return ([799a4ff0](http://github.com/fraywing/textAngular/commit/799a4ff0112c35cb68822eca10ff1a9f4250ab11))
* **taBind:** Fix paste issues ([f9d7e423](http://github.com/fraywing/textAngular/commit/f9d7e42336483da7376095fc1f741d6d0322a4df), closes [#407](http://github.com/fraywing/textAngular/issues/407))
* **taExecCommand:** Fix List conversion bug. ([d97842c6](http://github.com/fraywing/textAngular/commit/d97842c6696544e6971fcfda64ad91de908e79be), closes [#399](http://github.com/fraywing/textAngular/issues/399))


<a name="1.3.0-pre14"></a>
### 1.3.0-pre14 (2014-11-11)


#### Features

* **taTools:** Toggle HTML now uses code symbol from Font-Awesome ([856b31c3](http://github.com/fraywing/textAngular/commit/856b31c3f77716452a8e5d1d086e12db7934b43f), closes [#381](http://github.com/fraywing/textAngular/issues/381))
* **textAngular:**
  * Allow show html/code view by default, attribute ta-show-html. ([abf7bfb2](http://github.com/fraywing/textAngular/commit/abf7bfb28126928d8a5c8094ce90a0536752c97b))
  * Name is available on editor scope as `_name` ([6f03d559](http://github.com/fraywing/textAngular/commit/6f03d5593deb11f1dda5f485d069e007b91775fb), closes [#394](http://github.com/fraywing/textAngular/issues/394))


<a name="1.3.0-pre13"></a>
### 1.3.0-pre13 (2014-11-11)


#### Bug Fixes

* **$animation:** Fix angular 1.3.x compatability. ([b74ddf61](http://github.com/fraywing/textAngular/commit/b74ddf61d8a0864621b37224b9f02f6e5e74b25a), closes [#401](http://github.com/fraywing/textAngular/issues/401))
* **placeholder:** Fix the IE 11 bug with CSS style insert ([8e9e6625](http://github.com/fraywing/textAngular/commit/8e9e662574ac6302a3c9fb8cb2e572f3863dea89), closes [#390](http://github.com/fraywing/textAngular/issues/390))
* **taExecCommand:**
  * Fixes issue with list buttons and multiple lists. ([76815cbf](http://github.com/fraywing/textAngular/commit/76815cbf26bf8d3c20f7d60e1ef64763ac40effc), closes [#399](http://github.com/fraywing/textAngular/issues/399))
  * Add default wrap option to formatBlock ([c0fad4d9](http://github.com/fraywing/textAngular/commit/c0fad4d9a3c58cdbcb07c17f1c6876ae9305ab6b), closes [#400](http://github.com/fraywing/textAngular/issues/400))


<a name="1.3.0-pre12"></a>
### 1.3.0-pre12 (2014-11-04)


#### Bug Fixes

* **bower:** Fix files in main bower definition. ([00954faf](http://github.com/fraywing/textAngular/commit/00954faf43f583a81e079665f795058a099882eb), closes [#382](http://github.com/fraywing/textAngular/issues/382))
* **taBind:** Fixes paste nested list from word issues ([43bc8d9d](http://github.com/fraywing/textAngular/commit/43bc8d9d113e2379bea90c192405e4bb278c8ad9))
* **taExecCommand:** Fixes blockquote issue. ([63480a67](http://github.com/fraywing/textAngular/commit/63480a67d5bca3d91c5e5aae5abcd49e95a5ffe4), closes [#377](http://github.com/fraywing/textAngular/issues/377))


#### Features

* **taBind:** Press enter to escape a blockquote ([717c291c](http://github.com/fraywing/textAngular/commit/717c291cd0f23b8311cae5e0201a864b50861120))


<a name="1.3.0-pre11"></a>
### 1.3.0-pre11 (2014-10-31)


#### Bug Fixes

* **taBind:** Fix for only inline elements like `img` ([7123785f](http://github.com/fraywing/textAngular/commit/7123785fe400130f3a9f4e7469aadca4c94534df))
* **taExecCommand:** Fixes bug with blockquotes. ([5edb37cf](http://github.com/fraywing/textAngular/commit/5edb37cf3d8a2f537139401365bd06e22db97b16))


<a name="1.3.0-pre10"></a>
### 1.3.0-pre10 (2014-10-30)


#### Bug Fixes

* **taBind:**
  * Fix paste from word issue with nested lists and different margin measurements. ([20c4ea2e](http://github.com/fraywing/textAngular/commit/20c4ea2efcce918e35c9229f3f15bfce85889ba1))
  * Issue with unwrapped/empty content. ([be883684](http://github.com/fraywing/textAngular/commit/be8836840c2bb964537f329428e056a528eff8d2))
* **textAngularSetup:** Fix wordcount and charcount display with large numbers. ([42f1e349](http://github.com/fraywing/textAngular/commit/42f1e349374cef7d67cc60e257e2e9eec70defeb))


<a name="1.3.0-pre9"></a>
### 1.3.0-pre9 (2014-10-24)


#### Bug Fixes

* **compile:** Keep copyright notices in minified files ([9fe51ab6](http://github.com/fraywing/textAngular/commit/9fe51ab68a1b2d31528abc0fbee186c9e70b0698))
* **styling:** Support other CSS frameworks. ([280522a3](http://github.com/fraywing/textAngular/commit/280522a3daa4ec4a62710a98ce6ef5e2a662878a))
* **taBind:** Fixes paste lists, more lenient stripping of spans. ([5ff572f6](http://github.com/fraywing/textAngular/commit/5ff572f6c50d2bf68df0c2b729a0f224b2be78a1))
* **taExecCommand:** Attempt to wrap unwrapped content in list breaks. ([7b873df8](http://github.com/fraywing/textAngular/commit/7b873df8e4c58d4b62962b136eb598984d17d1e9))


<a name="1.3.0-pre8"></a>
### 1.3.0-pre8 (2014-10-23)


#### Bug Fixes

* **taBind:** Fix some paste from word issues. ([ca8af8b1](http://github.com/fraywing/textAngular/commit/ca8af8b17a363a9b70d63b1ebf5115ecb53b55c1))


<a name="1.3.0-pre7"></a>
### 1.3.0-pre7 (2014-10-22)


#### Bug Fixes

* **Setup:** Make the rangy loaded check more forgiving. ([ec778431](http://github.com/fraywing/textAngular/commit/ec7784311bc7256b0d216cd2b8a0321c897dd43b))


<a name="1.3.0-pre6"></a>
### 1.3.0-pre6 (2014-10-21)


#### Bug Fixes

* **taBind:** Fix the drop handler not re-applying on select handler ([af233b9f](http://github.com/fraywing/textAngular/commit/af233b9f2443c386afe9f83c5b1b2cd69d62e39d))
* **taExecCommand:** Fix lists for FF specifically. ([0924a8ca](http://github.com/fraywing/textAngular/commit/0924a8ca22493f018b679cc6a0805f8f1152f832), closes [#290](http://github.com/fraywing/textAngular/issues/290))
* **taSanitize:** Allow id attribute. ([7afc96c0](http://github.com/fraywing/textAngular/commit/7afc96c0896a60cec4d95099d172f7bfa37ed7a1), closes [#355](http://github.com/fraywing/textAngular/issues/355))
* **taTranslations:** Change Constant to Value ([58781ee9](http://github.com/fraywing/textAngular/commit/58781ee907a690c3f1e980c76ac71d67fb2187a6))


#### Features

* **taBind.undoManager:** Add undoManager to taBind. ([bd2bb0ae](http://github.com/fraywing/textAngular/commit/bd2bb0aee69953f5caa043571b854219a28145d0))


<a name="1.3.0-pre5"></a>
### 1.3.0-pre5 (2014-10-20)


#### Bug Fixes

* **bower:** Fixes angular bower dependancy to support 1.3.0 ([491c8daf](http://github.com/fraywing/textAngular/commit/491c8daf31078ccb38e02f2058bf2e5acbe7c4c9), closes [#358](http://github.com/fraywing/textAngular/issues/358))


#### Features

* **taBind:** Add paste from word converting. ([e9edbdfe](http://github.com/fraywing/textAngular/commit/e9edbdfe7376f28bc27a376ce15a61a6e14b2b81))


<a name="1.3.0-pre4"></a>
### 1.3.0-pre4 (2014-10-06)


#### Bug Fixes

* **taTools:** Fixes the wordcount to count correctly. ([fb208874](http://github.com/fraywing/textAngular/commit/fb208874a53abd2bea7c4f7fedd260dcee489141))


<a name="1.3.0-pre3"></a>
### 1.3.0-pre3 (2014-10-06)


#### Bug Fixes

* **taTools:**
	* If disabled is a value, respect it
	* Fix align active state when Justify / Full
	* Cleaned Up character count and stopped it from counting \n and \n\r linebreak characters.
* **taBind:** Fixes a list bug
* **IE/Paste:** More IE paste fixes.
* **fileDropHandler:** Fixes non-binding and long running file drop handlers not updating the model

<a name="1.3.0-pre2"></a>
### 1.3.0-pre2 (2014-10-06)


#### Bug Fixes

* **taExecCommand:** Shim the insertHTML function

#### Features

* **taTools:**
	* Add option to override default class
	* New word and character count tools.
	* Youtube videos now default to poster image from youtube API

<a name="1.3.0-pre1"></a>
### 1.3.0-pre1 (2014-10-06)


#### Bug Fixes

* **taBind:**
	* Validation on just whitespace
	* Ignoring keyup event on unnecessary keys
	* Remove Isolate Scope
* **window.event:** Window.event is undefined on FF
* **taExecCommand:** Collapsed selection creates link with url
* **taTools:** Fix clear collapsed list selection
* **animations:** Disable animations while switching views
* **paste:** Allow pasting of styles and random trash into the editor by sanitizing the paste event

#### Features

* **taSelection:** Add selection function
* **taSanitize:** Add background-color to accepted style options
* **taTools:** Add Strikethrough tool
* **CSP Compliance:** TextAngular is now CSP Compiant


###OLD Changelog - PRE v1.3.0-pre1

2014-07-26 v1.2.2

- FIX #190, #201, #206, #223, #224, 
- Merge #209, #204
- Add option to disable sanitizer #233

2014-05-19 v1.2.1

- Release

2014-05-12 v1.2.1-pre6

- FIX some FormatBlock issues.
- Add .ta-bind class to the ta-bind directive.

2014-05-01 v1.2.1-pre5

- ADD Included some css built into the editor - no need for extra stylesheets unless you want to override.
- CHANGE The registerTools function to be the entire signature so directives can be included as wanted.
- ADD resizeOverlay functionality, includes a new scroll window that the ta-text editor nests inside to make positioning better (TODO: tests).
- FIX ta-default-wrap in chrome bug.
- ADD Class .ta-bind to all ta-bind directive elements.
- FIX ta-default-wrap and other funkyness with ul/ol tags, #155.
- FIX some execCommand bugs by adding taExecCommand.

2014-04-08 v1.2.1-pre4

- Fixing IE bugs with ta-default-wrap.

2014-04-08 v1.2.1-pre3

- Fixing a change focus bug introduced in v1.2.1-pre2
- Changing the code so ta-bind no longer requires rangy-core.js, making it an optional requirement again.

2014-04-08 v1.2.1-pre2

- Fixed up ta-default-wrap. This now requires rangy-core.js
- Fixed an IE Paste issue.
- Fixed a webkit bug causing contenteditables not to loose focus.

2014-03-24 v1.2.1-pre1

- Moved setup functions into a seperate file, textAngularSetup.js. This file must be included before textAngular.js file. Using the defaults and textAngular.min.js causes no changes.
- Adding the Image and Link click popup functions.
- Adding ability to drag and drop files into the editor.
- Manager now can add and remove tools dynamically.
- Added Custom Renderers adding the ability to use placeholders, eg an image, in the editor and display something else in display mode. Uses factory function `taApplyCustomRenderers` to do this.

2014-02-28 v1.2.0

- Lots and Lots of changes, too many to list. Structural changes and added functionality. Supports down to IE8 and all other browsers.

2013-12-11 v1.1.2

- Updated to work correctly with IE (console.log bug)

2013-12-11 v1.1.2-pre3

- Added support for .focussed class and ng-focus to allow dynamic styling on focus events. #47
- Updates to fix Angular.JS breaking with parameter renaming minification. #49
- Minor bug fix to disable links from being 'clickable' in the editor.
- Updated the default toolbar to include ALL default tools.
- Update the tools to use activeState better.
- Small update to allow use of ta-bind outside of textAngular.
- Changed the raw html view to use a text-area for better compatability.

2013-12-09 v1.1.2-pre2

- Added input for form submission. #43
- Slight restructure and update into of /demo.
- Moved a lot of the README.md to the online Wiki. #34
- Changed pre-release tag names to -preX as we aren't really doing alpha - beta - RC format.

2013-12-05 v1.1.2-alpha (v1.1.2-pre1)

- Added bundled demo pages.
- Fixed Escaping of < and > #30
- Fixed stripping of style and class attributes and other parsing issues whilst maintaining the chrome fixes. #35 #30 #5
- Fixed two-way-binding not working #38
- Updated Readme.md and consolidated the readme out of the textAngular.js file.

2013-12-2 v1.1.1

- Fixed buttons still submitting form. #29
- Fix for Null ngModel value. Thanks to @slobo #22
- Added Ability to override just "display" for default button set. Thanks to @slobo #27

2013-11-9 v1.1.0

- Re-written to only depend on Angular and Angular-Sanitize. No More jQuery.
- Re-worked to be more angular-esq in it's initiation and use. Less reliance on global variables except for defaults and more use of bindings on attributes.
- Default styles are Bootstrap 3 classes, options to change these classes.
- Restructured the Toolbar to make it more plugin friendly, all tool buttons are encapsulated in their own scope that is a child of the individual textAngular bound scope.

2013-11-6 v1.0.3

- $sce isn't required anymore* Thanks to @nadeeshacabral
- bower support added* Thanks to @edouard-lopez

2013-10-11 v1.0.2

- Fixed issue with images not calling the compileHTML method*
- Fixed issue in chrome where styling was getting added for unordered lists*
- You can now change the model from the outside and have it affect the textAngular instance contents*
- Cleaned up code*

2013-10-10 v1.0.1 

- Added Tooltip Option, title has been renamed icon, and title is now the tooltip*
- The minified version actually works now*
