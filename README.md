# Pragma Historic

The Pragma Module for handling models changelogs in Pragma Framework.

## Installation

In composer.json add:

	require {"pragma-framework/historic": "dev-master"}

And in scripts blocks:

	"scripts": {
		"post-install-cmd": [
			"Pragma\\Historic\\Helpers\\Migrate::postInstallCmd"
		],
		"post-update-cmd": [
			"Pragma\\Historic\\Helpers\\Migrate::postUpdateCmd"
		]
	}

## What about created_at and created_by

These columns should be handled by within the PRAGMA_HISTORIC_CREATION_HOOK constant (in the config.php)
