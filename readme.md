# Lead Engineer Test

Given the following array:

```
$strings = [
	
	'Some random string that also has this string: [soundcloud url="https://api.soundcloud.com/tracks/910291" params="auto_play=false&amp;hide_related=false&amp;show_comments=true&amp;show_user=true&amp;show_reposts=false&amp;visual=true" width="100%" height="450" iframe="true" /] in it.',
	
	'Another completely random string that also has this string: [soundcloud url="https://api.soundcloud.com/tracks/5678?secret=test" params="auto_play=false&amp;hide_related=false&amp;show_comments=true&amp;show_user=true&amp;show_reposts=false&amp;visual=true" width="100%" height="450" iframe="true" /] in it test .',

	'Something else completely random string that also has this string: [soundcloud url="https://api.soundcloud.com/tracks/12345?secret=test" params="auto_play=false&amp;hide_related=false&amp;show_comments=true&amp;show_user=true&amp;show_reposts=false&amp;visual=true" width="100%" height="450" iframe="true" /] in i112222t.']'
];
```

Please complete the following questions:

#1 - Complete the excercise in PHP:

- In the array above, search for the following string: `[soundcloud url="{url-here}" params="auto_play=false&amp;hide_related=false&amp;show_comments=true&amp;show_user=true&amp;show_reposts=false&amp;visual=true" width="100%" height="450" iframe="true" /]`

- When you find this string, replace it with the following string: `[different-embed src="{different-url-here}"]`

- Before you do the replacement, please replace `{url-here}` with the corresponding value `{different-url-here}` from the CSV file in `data.csv` in this repo.

- The output from your code should be an array with the strings from `$strings` replaced with the new shortcode.  For example,

*BEFORE*
```
$strings[0] = 'Some random string that also has this string: [soundcloud url="https://api.soundcloud.com/tracks/910291" params="auto_play=false&amp;hide_related=false&amp;show_comments=true&amp;show_user=true&amp;show_reposts=false&amp;visual=true" width="100%" height="450" iframe="true" /] in it.';
```

*AFTER*
```
$strings[0] = 'Some random string that also has this string: [different-embed src="https://api.different-embed.com/12345"] in it.';
```

#2 - Please complete the same exact excercise, but in JavaScript.

#3 - Please package up your PHP command from task `#1` into a WordPress plugin that can be activated.  When the plugin is activated, it enables a wp-cli command that returns the updated `$strings` array after doing the search and replace.



