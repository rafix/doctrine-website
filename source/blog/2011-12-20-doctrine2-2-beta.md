---
title: "Doctrine 2.2 Beta"
menuSlug: blog
layout: blog-post
controller: ['Doctrine\Website\Controllers\BlogController', 'view']
authorName: Benjamin Eberlei
authorEmail:
categories: []
permalink: /2011/12/20/doctrine2-2-beta.html
---
We are proud to announce the start of the beta phase of Doctrine 2.2. I
think we implemented a nice amount of new features and refactored lots
of the code-base for simplicity and performance. Additionally we found a
bunch of new developers that contributed considerable amount of code.

A top list of the changes includes:

-   Filtering entities and associations based on rules that can be
    parameterized, enabled or disabled, developed by asm89
-   Support for complex SQL types such as Geometries, IPs, develped by
    jsor.
-   Bit Comparisions in DQL, developed by Fabio.
-   Annotation Refactorings by Fabio and johannes.
-   DQL Refactoring, ORDER BY and GROUP BY supporting result variables
    of SELECT expressions.
-   Alias for entities in DQL results.
-   Result Cache refactoring
-   Flush for single entities

See the changelogs of all three projects Common, DBAL, ORM:

-   [ORM](http://www.doctrine-project.org/jira/browse/DDC/fixforversion/10157)
-   [DBAL](http://www.doctrine-project.org/jira/browse/DBAL/fixforversion/10142)
-   [Common](http://www.doctrine-project.org/jira/browse/DCOM/fixforversion/10152)

In the next weeks will stabilize this code and add documentation for all
the new features. Additionally we try to drive the bug count down in the
2.1 branch as well.

Please test this beta with your projects to find any incompatibilities.
See the
[UPGRADE\_2\_2](https://github.com/doctrine/doctrine2/blob/master/UPGRADE_TO_2_2)
file to see backwards incompatible changes.

You can install the Beta through
[Github](https://github.com/doctrine/doctrine2) , \`PEAR
[http://pear.doctrine-project.org](http://pear.doctrine-project.org)\>\`\_
or through [Composer](http://www.packagist.org):

> {
> :   "require": { "doctrine/orm": "2.2.0-BETA1" }
>
> }
