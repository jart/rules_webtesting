<!---
Documentation generated by Skydoc
-->

# //web:repositories.bzl

Defines external repositories needed by rules_webtesting.

<nav class="toc">
  <h2>Macros</h2>
  <ul>
    <li><a href="#web_test_repositories">web_test_repositories</a></li>
    <li><a href="#browser_repositories">browser_repositories</a></li>
  </ul>
</nav>
<a name="web_test_repositories"></a>

## web_test_repositories

<pre>
web_test_repositories(<a href="#web_test_repositories.java">java</a>, <a href="#web_test_repositories.go">go</a>, <a href="#web_test_repositories.python">python</a>, <a href="#web_test_repositories.omit_com_github_gorilla_mux">omit_com_github_gorilla_mux</a>, <a href="#web_test_repositories.omit_org_seleniumhq_java">omit_org_seleniumhq_java</a>, <a href="#web_test_repositories.omit_com_google_code_findbugs_jsr305">omit_com_google_code_findbugs_jsr305</a>, <a href="#web_test_repositories.omit_com_google_guava_guava">omit_com_google_guava_guava</a>, <a href="#web_test_repositories.omit_com_github_tebeka_selenium">omit_com_github_tebeka_selenium</a>, <a href="#web_test_repositories.omit_org_seleniumhq_py">omit_org_seleniumhq_py</a>)
</pre>

Configure repositories for Web Test Launcher and for client languages.

<a name="web_test_repositories_args"></a>

### Attributes

<table class="params-table">
  <colgroup>
    <col class="col-param" />
    <col class="col-description" />
  </colgroup>
  <tbody>
    <tr id="web_test_repositories.java">
      <td><code>java</code></td>
      <td>
        <p><code>Boolean; Optional</code></p>
        <p>Configure Java client-side libraries.</p>
      </td>
    </tr>
    <tr id="web_test_repositories.go">
      <td><code>go</code></td>
      <td>
        <p><code>Boolean; Optional</code></p>
        <p>Configure Go client-side libraries.</p>
      </td>
    </tr>
    <tr id="web_test_repositories.python">
      <td><code>python</code></td>
      <td>
        <p><code>Boolean; Optional</code></p>
        <p>Configure Python client libraries.</p>
      </td>
    </tr>
    <tr id="web_test_repositories.omit_com_github_gorilla_mux">
      <td><code>omit_com_github_gorilla_mux</code></td>
      <td>
        <p><code>Boolean; Optional</code></p>
        <p>Do not install Gorilla MUX. Gorilla
MUX is required to compile the test launcher.</p>
      </td>
    </tr>
    <tr id="web_test_repositories.omit_org_seleniumhq_java">
      <td><code>omit_org_seleniumhq_java</code></td>
      <td>
        <p><code>Boolean; Optional</code></p>
        <p>Do not install Java Selenium client bindings.
These bindings are only installed if java=True.</p>
      </td>
    </tr>
    <tr id="web_test_repositories.omit_com_google_code_findbugs_jsr305">
      <td><code>omit_com_google_code_findbugs_jsr305</code></td>
      <td>
        <p><code>Boolean; Optional</code></p>
        <p>Do not install JSR305 annotations
library. This library is only installed if java=True.</p>
      </td>
    </tr>
    <tr id="web_test_repositories.omit_com_google_guava_guava">
      <td><code>omit_com_google_guava_guava</code></td>
      <td>
        <p><code>Boolean; Optional</code></p>
        <p>Do not install Guava libraries. This
library is only installed if java=True.</p>
      </td>
    </tr>
    <tr id="web_test_repositories.omit_com_github_tebeka_selenium">
      <td><code>omit_com_github_tebeka_selenium</code></td>
      <td>
        <p><code>Boolean; Optional</code></p>
        <p>Do not install Go WebDriver client
bindings. These binding are only installed if go=True.</p>
      </td>
    </tr>
    <tr id="web_test_repositories.omit_org_seleniumhq_py">
      <td><code>omit_org_seleniumhq_py</code></td>
      <td>
        <p><code>Boolean; Optional</code></p>
        <p>Do not install Python Selenium client bindings.
These bindings are only installed if python=True.</p>
      </td>
    </tr>
  </tbody>
</table>

<a name="browser_repositories"></a>

## browser_repositories

<pre>
browser_repositories(<a href="#browser_repositories.firefox">firefox</a>, <a href="#browser_repositories.chromium">chromium</a>, <a href="#browser_repositories.phantomjs">phantomjs</a>)
</pre>

Sets up repositories for browsers defined in //browsers/....

This should only be used on an experimental basis; projects should define their
own browsers.

<a name="browser_repositories_args"></a>

### Attributes

<table class="params-table">
  <colgroup>
    <col class="col-param" />
    <col class="col-description" />
  </colgroup>
  <tbody>
    <tr id="browser_repositories.firefox">
      <td><code>firefox</code></td>
      <td>
        <p><code>Boolean; Optional</code></p>
        <p>Configure repositories for //browsers:firefox-native.</p>
      </td>
    </tr>
    <tr id="browser_repositories.chromium">
      <td><code>chromium</code></td>
      <td>
        <p><code>Boolean; Optional</code></p>
        <p>Configure repositories for //browsers:chromium-native.</p>
      </td>
    </tr>
    <tr id="browser_repositories.phantomjs">
      <td><code>phantomjs</code></td>
      <td>
        <p><code>Boolean; Optional</code></p>
        <p>Configure repositories for //browsers:phantomjs-native.</p>
      </td>
    </tr>
  </tbody>
</table>