# VS-code
VS code 단축키와 스니펫 리스트입니다.

이에 대한 자세한 설명은 [제 블로그 포스트](https://assaeunji.github.io/etc/2020-05-07-snippets/)를 확인하세요!

## 단축키


| **`Ctrl` 기본 단축키**       | 설명     |
| :----------- | :----- |
| `Ctrl + Z`   | 되돌리기   |
| `Ctrl + X`   | 자르기    |
| `Ctrl + C`   | 복사하기   |
| `Ctrl + V`   | 붙여넣기   |
| `Ctrl + A`   | 전체선택   |
| `Ctrl + S`   | 저장     |
| `Ctrl + O`   | 파일 열기  |
| `Ctrl + W`   | 탭 닫기   |
| `Ctrl + Tab` | 탭 간 이동 |
| `Ctrl + P`   | 파일 찾기  |
| **`Ctrl` 마크다운  단축키**  | 설명                  |
| `Ctrl + B` | **B**old 체          |
| `Ctrl + I` | **I**talic 체        |
| `Ctrl + M` | **M**ath 수식 ($$) 적용 |
| **`Ctrl` 화살표 단축키**             | 설명       |
| `Ctrl + Up/Down`    | 스크롤      |
| `Ctrl + Left/Right` | 단어 단위 이동 |
| **`Ctrl` 찾기 삼형제 단축키** | 설명          |
| `Ctrl + F` | 찾기          |
| `Ctrl + H` | 찾고 바꾸기      |
| `Ctrl + D` | 단어 찾고 다중 커서 |
| **`Shift` 단축키**                  | 설명                           |
| `Shift + Left/Right`         | 한 **음절**씩 드래그                |
| `Ctrl + Shift + Left/ Right` | 한 **단어**씩 드래그                |
| `Shift + Up/Down`            | 한 **줄**씩 드래그                 |
| `Alt + Shift + Up/Down `     | 한 **문장** 복사 & 붙여넣기 |
| **`Alt` 단축키**          | 설명                    |
| `Alt + Left/Right` | 한 문장의 맨 앞, 맨 뒤로 커서 이동 |
| `Alt + Up / Down`  | 한 문장 / bullet 위치 이동 |

## 스니펫

<details>
<summary>펼쳐보기 (이대로 복사 붙여넣기 가능)</summary>
<div markdown="1">
<br/>

```json
{
	"@main":{
		"prefix": "@main",
		"body":[
			"---",
			"layout: post",
			"title:$1", 
			"date:", 
			"categories: []",
			"tag: []",
			"comments: true",
			"---",
		],
		"description": "make title"
	},
	"@sup":{
		"prefix": "@sup",
		"body":[
			"<sup>$1</sup>"
		],
		"description": "make superscript"
	},
	"@t":{
		"prefix": "@t",
		"body":[
			"---",
			"## $1"
		],
		"description": "make title"
	},
	"@st":{
		"prefix": "@st",
		"body":[
			"---",
			"### $1"
		],
		"description": "make subtitle"
	},
	"@sst":{
		"prefix": "@sst",
		"body":[
			":deciduous_tree: **$1**"
		],
		"description": "make subsubtitle"
	},
	"@img":{
		"prefix": "@img",
		"body":[
			"![](../../images/$1.png)"
		],
		"description": "put images"
	},
	"@link":{
		"prefix": "@link",
		"body":[
			"[`[link]`]($2)"
		],
		"description": "put link"
	},
	"@pdf":{
		"prefix": "@pdf",
		"body":[
			"[`[pdf]`]($2)"
		],
		"description": "put pdf"
	},
	"cpy":{
		"prefix": "cpy",
		"body":[
			"```python",
			"$1",
			"```"
		],
		"description": "make python cells"
	},
	"highyel":{
	"prefix": "highyel",
	"body":[
	"<mark style='background-color: #fff5b1'>$1</mark>"
	],
	"description": "highlight yellow"
	},
	"highred":{
	"prefix": "highred",
	"body":[
	"<mark style='background-color: #ffdce0'>$1</mark>"
	],
	"description": "highlight red"
	},
	"cred":{
	"prefix": "cred",
	"body":[
		"<font color='red'> $1 </font>"
	],
	"description": "red color"
	},
	"tab2":{
	"prefix": "@tab2",
	"body":[
     	"| $1  | $2  |",
		"|:---:|:---:|",
	],
	"description": "table with 2 columns"
	},
	"tab3":{
	"prefix": "@tab3",
	"body":[
     	"| $1  | $2  | $3  |",
		"|:---:|:---:|:---:|",
	],
	"description": "table with 3 columns"
	},
	"tab4":{
	"prefix": "@tab4",
	"body":[
     	"| $1  | $2  | $3  | $4  |",
		"|:---:|:---:|:---:|:---:|",
	],
	"description": "table with 4 columns"
	},
	"tab5":{
	"prefix": "@tab5",
	"body":[
     	"| $1  | $2  | $3  | $4  | $5  |",
		"|:---:|:---:|:---:|:---:|:---:|",
	],
	"description": "table with 5 columns"
	},
	"tab6":{
	"prefix": "@tab6",
	"body":[
     	"| $1  | $2  | $3  | $4  | $5  | $6  |",
		"|:---:|:---:|:---:|:---:|:---:|:---:|",
	],
	"description": "table with 6 columns"
	},
	"mathbbR": {
	"prefix": "@R",
	"body": [
	"\\mathbb{R}"
	],
	"description": "mathbb R"
	},
	"ulim": {
	"prefix": "Ulim",
	"body":[
	"\\underset{$1}{\\lim}"
	],
	"description": "underset limit"
	},
	"iid_sim":{
	"prefix": "iid",
	"body":[
	"\\overset{\\text{iid.}}{\\sim}"
	],
	"description": "iid over sim"
	},
	
	"ind_sim":{
	"prefix": "ind",
	"body":[
	"\\overset{\\text{ind.}}{\\sim}"
	],
	"description": "ind over sim"
	},
	"sum":{
	"prefix": "@sum",
	"body":[
	"\\sum_{$1=1}^{$2}"
	],
	"description": "summation"
	},
	"prod":{
	"prefix": "@prod",
	"body":[
	"\\prod_{$1=1}^{$2}"
	],
	"description": "product"
	},
	"xs":{
	"prefix": "xs",
	"body":[
	"$$x_1,\\ldots,x_n$ $0"
	],
	"description": "x_1 to x_n"
	},
	"int":{
	"prefix": "@int",
	"body":[
	"\\int_{$1}^{$2} $3\\mathrm{d}"	
	],
	"description": "integration"
	},
	"exp":{
	"prefix": "@exp",
	"body":[
	"\\mathrm{e}^{$1}"
	],
	"description": "exponential"
	},
	"min":{
	"prefix": "@min",
	"body":[
	"\\textrm{min}_{$1}"	
	],
	"description": "minimum"
	},
	"max":{
	"prefix": "@max",
	"body":[
	"\\textrm{max}_{$1}"	
	],
	"description": "maximum"
	},
	"BM": {
	"prefix": "@bm",
	"body": [
	"\\boldsymbol{$1}"
	],
	"description": "bold math"
	},
	"partial":{
	"prefix": "@fpa",
	"body":[
	"\\frac{\\partial $1}{\\partial $2}"
	],
	"description": "partial"
	},
	"dfrac":{
	"prefix": "@fd",
	"body":[
	"\\frac{\\mathrm{d} $1}{\\mathrm{d} $2}"
	],
	"description": "derivative"
	},
	"aligned":{
	"prefix": "@al",
	"body":[
	"$$",
	"\\begin{aligned}",
	"$1",
	"\\end{aligned}",
	"$$"
	],
	"description": "aligned"
	}
}
```

</div>
</details>
