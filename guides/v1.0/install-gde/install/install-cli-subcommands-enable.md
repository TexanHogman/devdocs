---
layout: default 
group: install 
subgroup: T_Command-line installation
title: Enable and disable modules
menu_title: Enable and disable modules
menu_node: 
menu_order: 5
github_link: install-gde/install/install-cli-subcommands-enable.md
---

  
#### Contents

*	<a href="#instgde-cli-subcommands-enable-disable">Module enable, disable</a>
*	<a href="#instgde-cli-subcommands-enable-modules">About enabling and disabling modules</a>


<h2 id="instgde-cli-subcommands-enable-disable">Module enable, disable</h2>
To enable or disable currently installed modules, use the following command:

	php index.php {module-enable|module-disable} {--modules="<list>"} [--force]

Use the following command to list enabled and disabled modules:

	php index.php help module-list

For example, to disable the Weee module, enter:

	php index.php module-disable --modules=Magento_Weee

<div class="bs-callout bs-callout-info" id="info">
<span class="glyphicon-class">
  <p>To enable or disable more than one module at a time, enter module names as a comma-separated list (no spaces).</p></span>
</div>

For important information about enabling and disabling modules, see <a href="#instgde-cli-subcommands-enable-modules">About enabling and disabling modules</a>.

<h2 id="instgde-cli-subcommands-enable-update">Update the database</h2>
If you enabled one or more modules, run the following command to update the database:

	php index.php update

<h2 id="instgde-cli-subcommands-enable-modules">About enabling and disabling modules</h2>
{% include install/enable-disable-modules.html %}

#### Related topics

*	<a href="{{ site.gdeurl }}install-gde/install/install-cli-install.html">Install the Magento software using the command line</a>
*	<a href="{{ site.gdeurl }}install-gde/install/install-cli-subcommands.html">Get started with the command-line installation</a>
*	<a href="{{ site.gdeurl }}install-gde/install/install-cli-subcommands-deployment.html">Create the deployment configuration, config.php</a>
*	<a href="{{ site.gdeurl }}install-gde/install/install-cli.html">Command line installation</a>