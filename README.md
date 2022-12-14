# ๐ฅถ KOLD: Korean Offensive Language Dataset
Repository for the KOLD dataset, paper accepted in [EMNLP 2022](https://2022.emnlp.org) (main, long).  
_Authors: [Younghoon Jeong](https://www.linkedin.com/in/boychaboy), [Juhyun Oh](https://www.linkedin.com/in/juhyun-oh-6839b9185/), [Jongwon Lee](https://www.linkedin.com/in/jongwon-jay-lee/), [Jaimeen Ahn](https://www.linkedin.com/in/jaimeenahn/), [Jihyung Moon](https://www.linkedin.com/in/mjihyung/), [Sungjoon Park](https://www.linkedin.com/in/sungjoon-park-815b6456/), and Alice Oh_  
_Institutions: KAIST, [Softly AI](https://softly.ai)_

**Note: This dataset must not be used as training data to automatically generate and publish offensive language online, but by publicly releasing it, we cannot prevent all malicious use. We do not condone any malicious use and urge researchers and practitioners to use it in beneficial ways (e.g., to filter out hate speech).**

## Paper
[KOLD: Korean Offensive Language Dataset](https://arxiv.org/abs/2205.11315) (arXiv version)  
_Camera-ready version link TBA_

### Illustration of Annotation Process
<img src="image/figure1.png" alt="Annotation Process" width="350"/>

### Examples of KOLD
<img src="image/table1.png" alt="Examples of KOLD" width="700"/>

### Target Group Attributes and Target Groups
<img src="image/table10.png" alt="Target Groups" width="700"/>

## Data
`data/kold_v1.json`
```
[
	{
		"guid": "kold-v1_00000",
		"source": "naver_news",
		"date": "2022-02-16",
		"title": "ํ๋ฏธ๋์ฆ์ด ๋ฒ์ฃ๊ฐ ๋๋ ๋๋ผ [์ถ๊ณผ ๋ฌธํ]",
		"comment": "๋จ๋ํ๋ฑ ์ฃผ์ฅํ  ๊ฑฐ๋ฉด ์ฌ์ฑ์ง๋ณ์ ์๋ ๋์ํ๋ผ๊ณ ใใใ ๊ทธ๋ฆฌ๊ณ  ๋ด ๋ง์ ๊ทธ๋ฅ ์๋น๋ง ๊ฑธ์ง ๋ง๊ณ  ํํ์ ๋ค ์ณ๋ฐ์ผ๋ฉด์ ์ ์ฐจ๋ณ๋ฐ๋๋ค๊ณ  ๋งํ๋์ง ๋งํด๋ณด๋ผ๊ณ ใใใ",
		"OFF": True,
		"TGT": "group",
		"GRP": "others-feminist",
		"OFF_span": " ์ณ๋ฐ์ผ๋ฉด์ ์ ์ฐจ๋ณ๋ฐ๋๋ค๊ณ  ๋งํ๋์ง ๋งํด๋ณด๋ผ๊ณ ใใใ"
		"TGT_span": ""
		"raw_labels": [
			  {'offensiveness': True,
			   'annotator_id': 191510,
			   'off_start_idx': [57],
			   'off_end_idx': [84],
			   'target': [['group']],
			   'target_group': [['์ง๋จ-์ฑ ์ ์ฒด์ฑ-์ฌ์ฑ']],
			   'tgt_start_idx': [],
			   'tgt_end_idx': []},
			  {'offensiveness': True,
			   'annotator_id': 192109,
			   'off_start_idx': [56],
			   'off_end_idx': [84],
			   'target': [['not specified', 'group']],
			   'target_group': [['์ง๋จ-์ฑ ์ ์ฒด์ฑ-ํ๋ฏธ๋์คํธ', '์ ์ ์์']],
			   'tgt_start_idx': [],
			   'tgt_end_idx': []},
			  {'offensiveness': True,
			   'annotator_id': 193299,
			   'off_start_idx': [0],
			   'off_end_idx': [84],
			   'target': [['group']],
			   'target_group': [['์ง๋จ-์ฑ ์ ์ฒด์ฑ-ํ๋ฏธ๋์คํธ']],
			   'tgt_start_idx': [],
			   'tgt_end_idx': [],}
			   ]
   	}
   ...
]
```
