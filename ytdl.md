> The 2021.12.17 release linked in the download instructions is now effectively obsolete; in particular, **it does not generally work with YouTube** itself. Before raising an issue, try a [nightly release build](#user-content-known_issues). But if you still need to raise an issue ...
> 
> Please **log in to GitHub before** using the 'New Issue' button.
> 
> Although 'New Issue' makes you log in, GitHub doesn't then show the template chooser that we set up to help you report issues. If you log in before using 'New Issue', you are correctly redirected to the chooser.
> 
> The chooser is [here](https://github.com/ytdl-org/youtube-dl/issues/new/choose). But **read on**, really.
> 
> If you raise an issue without using the chooser, or if you **ignore or misuse the chosen template**, your issue is likely either to be a duplicate of an issue that is already being handled, or to lack sufficient supporting information to solve the problem. Maintainers may close such issues without prejudice.
> 
> If your problem occurred when **running another package that invokes _youtube-dl_**, try to reproduce the problem with a `youtube-dl ...` command, or report it through the support channel for the other package; similarly if the problem occurred when running your own code.
> 
> If you are reporting an **error with diagnostic output** like this
> ```
> youtube_dl...SomeError: oops; please report this issue on https://yt-dl.org/bug ...
> ```
> do **follow the instructions** there, including, implicitly, this post.
> * Take note of the error message, `oops` in the example above.
> * The issue template will ask you to check for an existing issue that covers the error (but first review **'Known issues' [below](#user-content-known_issues)**):
>   - use something like `is:issue oops -label:duplicate` in the search field of the project issue tracker, where `oops` is the message that you noted before;
>   - add `-in:title` if the search returns too many results.
> * HTTP errors 4xx and 5xx and errors in data extraction are likely to be specific to a single site or extractor: for such errors, prioritise issues that match the site or extractor in your problem.
> * **Don't raise a new issue** if an existing issue matches your problem.
> * [Why is all this important for the project?](https://github.com/ytdl-org/youtube-dl/issues/32460#issuecomment-1645501634)
> * [Some German madness is temporarily breaking the domain yt-dl.org](https://github.com/ytdl-org/youtube-dl/issues/32495): until the name points to a valid domain, there is a revised version of the [README](https://github.com/ytdl-org/youtube-dl/blob/9324d03ef9cfd8e26874cead3a2c1b5c78cdb42c/README.md) (and the reporting URL is this tracker, but you're already here).
> * If you want a **version of _youtube_dl_ that can actually download from YouTube**, use a recent nightly build: see **'Known issues'** [below](#user-content-known_issues).
> 
> If you were actually **running _yt-dlp_**, go [there](https://github.com/yt-dlp/yt-dlp/issues). Similarly with other forks, unless code clearly matches the _youtube_dl_ release or git master code.
> 
> If your problem concerns `HTTP Error 429: Too Many Requests`, especially with YouTube or a video hosted there, **read #23638 and its linked issue first** to avoid having your issue closed immediately.
> 
> Although your issue may concern a site that uses a language other than English and/or English may not be your first language, please **formulate your issue in English**. Various online translation tools are available to help you, even [this](https://translate.google.com?tl=en). [By all means include your original text in case the automatic translation is defective](https://github.com/ytdl-org/youtube-dl/issues/31438#issuecomment-1364685812).
> 
> You can use the HTML `details` element to hide the original text, or to improve readability when posting multiple logs, etc:
> ```
> <details><summary>Original text</summary>
> 
> original text or other details here
> 
> </details>
> ```
> **<a id="known_issues">Known issues</a>**, fixed in git master code, or update/install from the [nightly release repo](https://github.com/ytdl-org/ytdl-nightly/releases/latest):
> * [YouTube: Unable to extract nsig jsi ...](https://github.com/ytdl-org/youtube-dl/issues/32842)
> * [YouTube: Error 403 when downloading ...](https://github.com/ytdl-org/youtube-dl/issues/32815))
> * [YouTube: Unable to extract yt initial data on playlist](https://github.com/ytdl-org/youtube-dl/issues/32499) (also a swathe of [related errors](https://github.com/ytdl-org/youtube-dl/issues/32499/linked_closing_reference?reference_location=REPO_ISSUES_INDEX)
> * [YouTube: Unable to extract uploader id](https://github.com/ytdl-org/youtube-dl/issues/31530)
> * [YouTube: Unable to decode n-parameter: download likely to be throttled](https://github.com/ytdl-org/youtube-dl/issues/31509)
> * [Vimeo: Unable to extract info section](https://github.com/ytdl-org/youtube-dl/issues/31311)
> * [YouTube: shorts URL causes "unable to recognize tab page" errors](https://github.com/ytdl-org/youtube-dl/issues/30269)
> * [YouTube: youtube-dl does not find videos listed on user/channel "shorts" subpage](https://github.com/ytdl-org/youtube-dl/issues/31336)
> * [ITVX support](https://github.com/ytdl-org/youtube-dl/issues/31363): (but new problems have been reported that are not yet resolved)
> * [YouTube: Signature extraction failed, KeyError QV](https://github.com/ytdl-org/youtube-dl/issues/32314)
> * [Security: File Downloader cookie leak](https://github.com/ytdl-org/youtube-dl/issues/31363)
