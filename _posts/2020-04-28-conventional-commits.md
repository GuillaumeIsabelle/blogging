---
ID: 1846
post_title: Conventional Commits
author: gicomadmin
post_excerpt: ""
layout: post
permalink: >
  http://guillaumeisabelle.com/blogging/2020/04/28/conventional-commits/
published: true
post_date: 2020-04-28 14:38:54
---
> Conventional Commits A specification for adding human and machine readable meaning to commit messages

Source: *[Conventional Commits][1]*

<!-- wp:paragraph -->

<http://afelia.jgwill.com/nc/1096>

<!-- /wp:paragraph -->

<!-- wp:atomic-blocks/ab-accordion {"accordionFontSize":24} -->

<div class="wp-block-atomic-blocks-ab-accordion ab-block-accordion ab-font-size-24">
  <details><summary class="ab-accordion-title">Specification</summary><div class="ab-accordion-text">
    <!-- wp:paragraph -->
    
    <p>
      The key words “MUST”, “MUST NOT”, “REQUIRED”, “SHALL”, “SHALL NOT”, “SHOULD”, “SHOULD NOT”, “RECOMMENDED”, “MAY”, and “OPTIONAL” in this document are to be interpreted as described in <a href="https://www.ietf.org/rfc/rfc2119.txt">RFC 2119</a>.
    </p>
    
    <!-- /wp:paragraph -->
    
    <!-- wp:list {"ordered":true} -->
    
    <ol>
      <li>
        Commits MUST be prefixed with a type, which consists of a noun, <code>feat</code>, <code>fix</code>, etc., followed by the OPTIONAL scope, OPTIONAL <code>!</code>, and REQUIRED terminal colon and space.
      </li>
      <li>
        The type <code>feat</code> MUST be used when a commit adds a new feature to your application or library.
      </li>
      <li>
        The type <code>fix</code> MUST be used when a commit represents a bug fix for your application.
      </li>
      <li>
        A scope MAY be provided after a type. A scope MUST consist of a noun describing a section of the codebase surrounded by parenthesis, e.g., <code>fix(parser):</code>
      </li>
      <li>
        A description MUST immediately follow the colon and space after the type/scope prefix. The description is a short summary of the code changes, e.g., <em>fix: array parsing issue when multiple spaces were contained in string</em>.
      </li>
      <li>
        A longer commit body MAY be provided after the short description, providing additional contextual information about the code changes. The body MUST begin one blank line after the description.
      </li>
      <li>
        A commit body is free-form and MAY consist of any number of newline separated paragraphs.
      </li>
      <li>
        One or more footers MAY be provided one blank line after the body. Each footer MUST consist of a word token, followed by either a <code>:&lt;space></code> or <code>&lt;space>#</code> separator, followed by a string value (this is inspired by the <a href="https://git-scm.com/docs/git-interpret-trailers">git trailer convention</a>).
      </li>
      <li>
        A footer’s token MUST use <code>-</code> in place of whitespace characters, e.g., <code>Acked-by</code> (this helps differentiate the footer section from a multi-paragraph body). An exception is made for <code>BREAKING CHANGE</code>, which MAY also be used as a token.
      </li>
      <li>
        A footer’s value MAY contain spaces and newlines, and parsing MUST terminate when the next valid footer token/separator pair is observed.
      </li>
      <li>
        Breaking changes MUST be indicated in the type/scope prefix of a commit, or as an entry in the footer.
      </li>
      <li>
        If included as a footer, a breaking change MUST consist of the uppercase text BREAKING CHANGE, followed by a colon, space, and description, e.g., <em>BREAKING CHANGE: environment variables now take precedence over config files</em>.
      </li>
      <li>
        If included in the type/scope prefix, breaking changes MUST be indicated by a <code>!</code> immediately before the <code>:</code>. If <code>!</code> is used, <code>BREAKING CHANGE:</code> MAY be committed from the footer section, and the commit description SHALL be used to describe the breaking change.
      </li>
      <li>
        Types other than <code>feat</code> and <code>fix</code> MAY be used in your commit messages, e.g., <em>docs: updated ref docs.</em>
      </li>
      <li>
        The units of information that make up Conventional Commits MUST NOT be treated as case sensitive by implementors, with the exception of BREAKING CHANGE which MUST be uppercase.
      </li>
      <li>
        BREAKING-CHANGE MUST be synonymous with BREAKING CHANGE, when used as a token in a footer.
      </li>
    </ol>
    
    <!-- /wp:list -->
  </div></details>
</div>

<!-- /wp:atomic-blocks/ab-accordion -->

<!-- wp:atomic-blocks/ab-accordion {"accordionFontSize":24,"accordionOpen":true} -->

<div class="wp-block-atomic-blocks-ab-accordion ab-block-accordion ab-font-size-24">
  <details open><summary class="ab-accordion-title">Why Use Conventional Commits</summary><div class="ab-accordion-text">
    <!-- wp:list -->
    
    <ul>
      <li>
        Automatically generating CHANGELOGs.
      </li>
      <li>
        Automatically determining a semantic version bump (based on the types of commits landed).
      </li>
      <li>
        Communicating the nature of changes to teammates, the public, and other stakeholders.
      </li>
      <li>
        Triggering build and publish processes.
      </li>
      <li>
        Making it easier for people to contribute to your projects, by allowing them to explore a more structured commit history.
      </li>
    </ul>
    
    <!-- /wp:list -->
  </div></details>
</div>

<!-- /wp:atomic-blocks/ab-accordion -->

 [1]: https://www.conventionalcommits.org/en/v1.0.0/