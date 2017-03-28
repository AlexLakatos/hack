---
layout: default
---

# Sign up

We'll be using a [central GitHub repository](https://github.com/jsoxford/hack) to keep everything in sync.  If you don't have a GitHub account - [sign up now](https://github.com).

__Note: if you're a multi-person team, only one of you should sign up.__

## Step 1.
### Enter some details
{: .sub-heading}

<form id="entry-form">
  <div class="field">
    <label for="name">Team name</label>
    <input type="text" name="name" id="name" placeholder="">
  </div>
  <div class="field">
    <label for="name">Members</label>
    <input type="text" name="members" id="members" placeholder="@github @user-names">
  </div>
  <div class="field">
    <label for="guide">Guide</label>
    <select name="guide" id="guide">
      {% for guide in site.data.guides %}
        <option value="{{ guide.github }}">{{ guide.name }} ({{ guide.technology }})</option>
      {% endfor %}
    </select>
  </div>
  <div class="field">
    <label for="description">Description <div><small>Markdown? Totes</small></div></label>
    <textarea name="description" id="description"></textarea>
  </div>
</form>


## Step 2.
### Create a file in the [GitHub](https://github.com/jsoxford/hack) project
{: .sub-heading}


<!-- ```
---
name: Team name
members:
  - username
guide: username
---

Your description here
``` -->


<div class="file-name" id="gh-filename">hacks/team-name.md</div>
<pre class="file-content"><code id="gh-content">---
name: Team name
members:
  - username
guide: username
---

Your description here</code></pre>

The easiest way to do this is through the GitHub editor:

<a href="#" id="gh-link">Click this link</a>



## Step 3.
### Open a Pull Request
{: .sub-heading}

One of our beautiful helpers will check & merge your PR.
