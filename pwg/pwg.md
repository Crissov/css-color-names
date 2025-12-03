PWG Media Color Names
=====================

[IEEE-ISTO 5101.1: PWG Media Standardized Names v2.1 (MSN)](https://ftp.pwg.org/pub/pwg/candidates/cs-pwgmsn21-20230915-5101.1.pdf)
claims that the media color names (and supposedly their values) found in Table 2 are based upon:

- Printer MIB v2 [[RFC3805] `prtInputMediaColor`](https://www.rfc-editor.org/rfc/rfc3805#page-88)
- [Job Ticket Application Programming Interface (JTAPI)](https://wiki.linuxfoundation.org/openprinting/jtapi)

but JTAPI only contains an associated [header file](ftp://ftp.pwg.org/pub/pwg/fsg/jobticket/C_JTAPI_Code/CJTAPI_22Apr2005.zip/fsgjt_enums.h)) with media color name enums without values
and RFC3805 refers back to [PWGMEDIA],
whereas the predecessor it replaces, [RFC1759](https://www.rfc-editor.org/rfc/rfc1759#page-44),
mentions a brief list of keywords without explicit color value:

 - `other`
 - `unknown`
 - `white`
 - `pink`
 - `yellow`
 - `buff`
 - `goldenrod`
 - `blue`
 - `green`
 - `transparent`

In any case, `transparent` equals `no-color` and is a fully transparent white, not black.
`Undefined` has been recorded as `none` (N/V) for completeness only.
`Clear` means 50% opacity of the unaltered base consistently.

| English Localized Name	| Name	| Base	| Clear `clear-`	| Dark `dark-`	| Light `light-`	|
| -----	| -----	| ---	| ---	| ---	| ---	|
| Transparent	| `no-color`| `#FFFFFF00`|   N/A    |   N/A    |   N/A    |
| Black	| `black`	| `#000000`| `#0000007F`|   N/A    | `#808080`|
| Blue	| `blue`	| `#0000FF`| `#0000FF7F`| `#00008B`| `#ADD8E6`|
| Brown	| `brown`	| `#A52A2A`| `#A52A2A7F`| `#5C4033`| `#9966FF`|
| Buff	| `buff`	| `#F0DC82`| `#F0DC827F`| `#976638`| `#ECD9B0`|
| Cyan	| `cyan`	| `#00FFFF`| `#00FFFF7F`| `#008B8B`| `#E0FFFF`|
| Gold	| `gold`	| `#FFD700`| `#FFD7007F`| `#EEBC1D`| `#F1E5AC`|
| Goldenrod	| `goldenrod`	| `#DAA520`| `#DAA5207F`| `#B8860B`| `#FFEC8B`|
| Gray	| `gray`	| `#808080`| `#8080807F`| `#404040`| `#D3D3D3`|
| Green	| `green`	| `#008000`| `#0080007F`| `#006400`| `#90EE90`|
| Ivory	| `ivory`	| `#FFFFF0`| `#FFFFF07F`| `#F2E58F`| `#FFF8C9`|
| Magenta	| `magenta`	| `#FF00FF`| `#FF00FF7F`| `#8B008B`| `#FF77FF`|
| Mustard	| `mustard`	| `#FFDB58`| `#FFDB587F`| `#7C7C40`| `#EEDD62`|
| Orange	| `orange`	| `#FFA500`| `#FFA5007F`| `#FF8C00`| `#D9A465`|
| Pink	| `pink`	| `#FFC0CB`| `#FFC0CB7F`| `#E75480`| `#FFB6C1`|
| Red	| `red`	| `#FF0000`| `#FF00007F`| `#8B0000`| `#FF3333`|
| Silver	| `silver`	| `#C0C0C0`| `#C0C0C07F`| `#AFAFAF`| `#E1E1E1`|
| Turquoise	| `turquoise`	| `#30D5C8`| `#30D5C87F`| `#00CED1`| `#AFE4DE`|
| Violet	| `violet`	| `#EE82EE`| `#EE82EE7F`| `#9400D3`| `#7A5299`|
| White	| `white`	| `#FFFFFF`| `#FFFFFF7F`|
| Yellow	| `yellow`	| `#FFFF00`| `#FFFF007F`| `#FFCC00`| `#FFFFE0`|
| Multi-Color	| `multi-color`	|   N/V    |   N/V    |   N/A    |   N/A    |
