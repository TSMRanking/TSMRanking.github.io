# TSM Ranking
Hello TSM Players, this is the **OFFICIAL RANKING WEBSITE** For TSM, Join our [Discord Server](https://discord.gg/touchsoccermultiverse) for more information
 
## How To Contribution?!:
To Contribution you have to understand the [Source Code](index.html), and im gonna show you how is it works:
- To Add a **Team** in the ranking, make sure to put this inside **currentGlobalRanking** function
```js
{ rank: 44, name: "Team 1", code: "TRS", points: 1000.00, change: "same", changeValue: 0, pointsChange: 0 }
```
- **rank** is the important thing, make sure to put the **rank** is a number and put it in the exact place for example if the rank was **45** then, add it under **Team 1**

- **code** is the country flag, to find the flag code make sure to check the **Team** or country code and here the list:
```js
                // european teams
                'ALB': 'al', 'AND': 'ad', 'ARM': 'am', 'AUT': 'at', 'AZE': 'az',
                'BEL': 'be', 'BIH': 'ba', 'BLR': 'by', 'BUL': 'bg', 'CRO': 'hr',
                'CYP': 'cy', 'CZE': 'cz', 'DEN': 'dk', 'ENG': 'gb-eng', 'ESP': 'es',
                'EST': 'ee', 'FIN': 'fi', 'FRA': 'fr', 'GEO': 'ge', 'GER': 'de',
                'GIB': 'gi', 'GRE': 'gr', 'HUN': 'hu', 'ISL': 'is', 'ISR': 'il',
                'ITA': 'it', 'KAZ': 'kz', 'KOS': 'xk', 'LVA': 'lv', 'LIE': 'li',
                'LTU': 'lt', 'LUX': 'lu', 'MLT': 'mt', 'MDA': 'md', 'MKD': 'mk',
                'MNE': 'me', 'NED': 'nl', 'NIR': 'gb-nir', 'NOR': 'no', 'POL': 'pl',
                'POR': 'pt', 'IRL': 'ie', 'ROU': 'ro', 'RUS': 'ru', 'SMR': 'sm',
                'SCO': 'gb-sct', 'SRB': 'rs', 'SVK': 'sk', 'SVN': 'si', 'SWE': 'se',
                'SUI': 'ch', 'TUR': 'tr', 'UKR': 'ua', 'WAL': 'gb-wls', 'FRO': 'fo',

                // south american teams
                'ARG': 'ar', 'BOL': 'bo', 'BRA': 'br', 'CHL': 'cl', 'COL': 'co',
                'ECU': 'ec', 'PAR': 'py', 'PER': 'pe', 'URY': 'uy', 'VEN': 've', 'SUR': 'sr',

                // north and central america teams
                'USA': 'us', 'CAN': 'ca', 'MEX': 'mx', 'CRC': 'cr', 'PAN': 'pa',
                'JAM': 'jm', 'HAI': 'ht', 'HON': 'hn', 'SLV': 'sv', 'TRI': 'tt',
                'GUY': 'gy', 'CUW': 'cw', 'GRN': 'gd', 'NCA': 'ni', 'DMA': 'dm', 'GTM': 'gt', 'MSR': 'ms', 'CYM': 'ky', 'DOM': 'do', 'SKN': 'kn', 'PUR': 'pr', 'ATG': 'ag', 'CUB': 'cu', 'LCA': 'lc', 'BER': 'bm', 'VIN': 'vc', 'BRB': 'bb', 'BLZ': 'bz', 'COK': 'ck', 'ARU': 'aw', 'VIR': 'vi', 'TCA': 'tc', 'BAH': 'bs', 'VGB': 'vg', 'AIA': 'ai',

                // african
                'ALG': 'dz', 'ANG': 'ao', 'BEN': 'bj', 'BFA': 'bf', 'BDI': 'bi', 'MWI': 'mw',
                'CMR': 'cm', 'CPV': 'cv', 'CTA': 'cf', 'TCH': 'td', 'COM': 'km',
                'CGO': 'cg', 'COD': 'cd', 'CIV': 'ci', 'DJI': 'dj', 'EGY': 'eg',
                'EQG': 'gq', 'ERI': 'er', 'ETH': 'et', 'GAB': 'ga', 'GAM': 'gm',
                'GHA': 'gh', 'GUI': 'gn', 'GNB': 'gw', 'KEN': 'ke', 'LES': 'ls',
                'LBR': 'lr', 'LBY': 'ly', 'MAD': 'mg', 'MLI': 'ml', 'MTN': 'mr',
                'MRI': 'mu', 'MAR': 'ma', 'MOZ': 'mz', 'NAM': 'na', 'NIG': 'ne',
                'NGA': 'ng', 'RWA': 'rw', 'STP': 'st', 'SEN': 'sn', 'SEY': 'sc',
                'SLE': 'sl', 'SOM': 'so', 'RSA': 'za', 'SSD': 'ss', 'SUD': 'sd',
                'SWZ': 'sz', 'TAN': 'tz', 'TOG': 'tg', 'TUN': 'tn', 'UGA': 'ug',
                'ZAM': 'zm', 'ZIM': 'zw', 'BWA': 'bw',

                // asian
                'AFG': 'af', 'AUS': 'au', 'BHR': 'bh', 'BAN': 'bd', 'BHU': 'bt',
                'BRU': 'bn', 'CAM': 'kh', 'CHN': 'cn', 'TPE': 'tw', 'HKG': 'hk',
                'IND': 'in', 'IDN': 'id', 'IRN': 'ir', 'IRQ': 'iq', 'JPN': 'jp',
                'JOR': 'jo', 'KAZ': 'kz', 'PRK': 'kp', 'KOR': 'kr', 'KUW': 'kw',
                'KGZ': 'kg', 'LAO': 'la', 'LBN': 'lb', 'MAC': 'mo', 'MAY': 'my',
                'MDV': 'mv', 'MGL': 'mn', 'MYA': 'mm', 'NEP': 'np', 'OMA': 'om',
                'PAK': 'pk', 'PLE': 'ps', 'PHI': 'ph', 'QAT': 'qa', 'KSA': 'sa',
                'SIN': 'sg', 'SRI': 'lk', 'SYR': 'sy', 'TJK': 'tj', 'THA': 'th',
                'TLS': 'tl', 'TKM': 'tm', 'UAE': 'ae', 'UZB': 'uz', 'VIE': 'vn',
                'YEM': 'ye',

                // oceania
                'ASA': 'as', 'FIJ': 'fj', 'NCL': 'nc', 'NZL': 'nz', 'SOL': 'sb',
                'TAH': 'pf', 'TGA': 'to', 'VAN': 'vu', 'SAM': 'ws', 'PNG': 'pg', 'GUM': 'gu',
```
Make sure to use the code that have all letters **BIG**

- **points** are the points for the team

- **change** shows if the team got ranked up, ranked down, still in their rank
  - **same** is the still in their rank like even after updates they still in their rank
  - **up** means the team promoted to a new rank
  - **down** means the team losed or demoted from their rank

- **changeValue** all the team need to have the value 1, we will edit that, because without changing it the **change** function will not work and up, down, will not appear, make sure before updating to check if **changeValue** value is 1

- **pointsChange** is the points that the team gained or losed, if it was + means it will be green text, if - then red text, if nothing but just numbers like 0.33 means green text

## About TSM Ranking:
- Made by GozF4x (Zakaria)
- Join our [Discord Server](https://discord.gg/touchsoccermultiverse)