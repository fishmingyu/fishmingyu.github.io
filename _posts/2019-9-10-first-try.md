---
layout: post
title: The first try
description: 2019北大综合营数学第5题
---
这是我作为一个新手第一次尝试用*GitHub Pages*的方法来构建个人主页。由于我本人是学电子的，对前端开发基本一概不知。感谢[thelehhman](https://github.com/thelehhman/texture)精心制作的网站内核。


<html>
<head>
  <meta charset='UTF-8'>
  <meta name='viewport' content='width=device-width initial-scale=1'>
  <meta name='description' content='2019'>
  <title>2019_peking_summercamp_math5</title>
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/katex@0.11.0/dist/katex.min.css"
    integrity="sha384-BdGj8xC2eZkQaxoQ8nSLefg4AV4/AwB3Fj+8SUSo7pnKP6Eoy18liIKTPn9oBYNG" crossorigin="anonymous">
  <!-- The loading of KaTeX is deferred to speed up page rendering -->
  <script defer src="https://cdn.jsdelivr.net/npm/katex@0.11.0/dist/katex.min.js"
    integrity="sha384-JiKN5O8x9Hhs/UE5cT5AAJqieYlOZbGT3CHws/y97o3ty4R7/O5poG9F3JoiOYw1"
    crossorigin="anonymous"></script>
</head>

<body>
  <h1>2019北大综合营数学第5题</h1>
  <blockquote>
    <p>题目：</p>
    <p>将10条长度为1的线段分成若干段，证明在得到的所有线段中一定可以找到6条线段，能够组成两个三角形。</p>
  </blockquote>
  <h3>分类一：<span class="MathJax_SVG" tabindex="-1" style="font-size: 100%; display: inline-block;"><svg
        xmlns:xlink="http://www.w3.org/1999/xlink" width="1.291ex" height="1.894ex" viewBox="0 -770.6 556 815.3"
        role="img" focusable="false" style="vertical-align: -0.104ex;">
        <defs>
          <path stroke-width="0" id="E3-MJMAIN-2203"
            d="M56 661T56 674T70 694H487Q497 686 500 679V15Q497 10 487 1L279 0H70Q56 7 56 20T70 40H460V327H84Q70 334 70 347T84 367H460V654H70Q56 661 56 674Z">
          </path>
        </defs>
        <g stroke="currentColor" fill="currentColor" stroke-width="0" transform="matrix(1 0 0 -1 0 0)">
          <use xlink:href="#E3-MJMAIN-2203" x="0" y="0"></use>
        </g>
      </svg></span>
    <script type="math/tex">{\exist}</script> 2及以上个线段，每个线段中均可以找出三条线段构成三角形</h3>
  <h3>分类二：仅 <span class="MathJax_SVG" tabindex="-1" style="font-size: 100%; display: inline-block;"><svg
        xmlns:xlink="http://www.w3.org/1999/xlink" width="1.291ex" height="1.894ex" viewBox="0 -770.6 556 815.3"
        role="img" focusable="false" style="vertical-align: -0.104ex;">
        <defs>
          <path stroke-width="0" id="E3-MJMAIN-2203"
            d="M56 661T56 674T70 694H487Q497 686 500 679V15Q497 10 487 1L279 0H70Q56 7 56 20T70 40H460V327H84Q70 334 70 347T84 367H460V654H70Q56 661 56 674Z">
          </path>
        </defs>
        <g stroke="currentColor" fill="currentColor" stroke-width="0" transform="matrix(1 0 0 -1 0 0)">
          <use xlink:href="#E3-MJMAIN-2203" x="0" y="0"></use>
        </g>
      </svg></span>
    <script type="math/tex">{\exist}</script> 1个线段，可以找出一个三角形</h3>
  <h3>分类三：<span class="MathJax_SVG" tabindex="-1" style="font-size: 100%; display: inline-block;"><svg
        xmlns:xlink="http://www.w3.org/1999/xlink" width="1.291ex" height="1.993ex" viewBox="0 -770.6 556 858"
        role="img" focusable="false" style="vertical-align: -0.203ex;">
        <defs>
          <path stroke-width="0" id="E4-MJMAIN-2200"
            d="M0 673Q0 684 7 689T20 694Q32 694 38 680T82 567L126 451H430L473 566Q483 593 494 622T512 668T519 685Q524 694 538 694Q556 692 556 674Q556 670 426 329T293 -15Q288 -22 278 -22T263 -15Q260 -11 131 328T0 673ZM414 410Q414 411 278 411T142 410L278 55L414 410Z">
          </path>
        </defs>
        <g stroke="currentColor" fill="currentColor" stroke-width="0" transform="matrix(1 0 0 -1 0 0)">
          <use xlink:href="#E4-MJMAIN-2200" x="0" y="0"></use>
        </g>
      </svg></span>
    <script type="math/tex">{\forall}</script> 线段中均不能从自身中找出三角形</h3>
  <h2>证明</h2>
  <blockquote>
    <p>引理：对于一个不能从自身找出三角形的线段，一定会有一根线段长度<span class="MathJax_SVG" tabindex="-1"
        style="font-size: 100%; display: inline-block;"><svg xmlns:xlink="http://www.w3.org/1999/xlink" width="5.936ex"
          height="2.671ex" viewBox="0 -835.3 2555.8 1149.8" role="img" focusable="false"
          style="vertical-align: -0.73ex;">
          <defs>
            <path stroke-width="0" id="E18-MJMAIN-2265"
              d="M83 616Q83 624 89 630T99 636Q107 636 253 568T543 431T687 361Q694 356 694 346T687 331Q685 329 395 192L107 56H101Q83 58 83 76Q83 77 83 79Q82 86 98 95Q117 105 248 167Q326 204 378 228L626 346L360 472Q291 505 200 548Q112 589 98 597T83 616ZM84 -118Q84 -108 99 -98H678Q694 -104 694 -118Q694 -130 679 -138H98Q84 -131 84 -118Z">
            </path>
            <path stroke-width="0" id="E18-MJMAIN-31"
              d="M213 578L200 573Q186 568 160 563T102 556H83V602H102Q149 604 189 617T245 641T273 663Q275 666 285 666Q294 666 302 660V361L303 61Q310 54 315 52T339 48T401 46H427V0H416Q395 3 257 3Q121 3 100 0H88V46H114Q136 46 152 46T177 47T193 50T201 52T207 57T213 61V578Z">
            </path>
            <path stroke-width="0" id="E18-MJMAIN-2F"
              d="M423 750Q432 750 438 744T444 730Q444 725 271 248T92 -240Q85 -250 75 -250Q68 -250 62 -245T56 -231Q56 -221 230 257T407 740Q411 750 423 750Z">
            </path>
            <path stroke-width="0" id="E18-MJMAIN-33"
              d="M127 463Q100 463 85 480T69 524Q69 579 117 622T233 665Q268 665 277 664Q351 652 390 611T430 522Q430 470 396 421T302 350L299 348Q299 347 308 345T337 336T375 315Q457 262 457 175Q457 96 395 37T238 -22Q158 -22 100 21T42 130Q42 158 60 175T105 193Q133 193 151 175T169 130Q169 119 166 110T159 94T148 82T136 74T126 70T118 67L114 66Q165 21 238 21Q293 21 321 74Q338 107 338 175V195Q338 290 274 322Q259 328 213 329L171 330L168 332Q166 335 166 348Q166 366 174 366Q202 366 232 371Q266 376 294 413T322 525V533Q322 590 287 612Q265 626 240 626Q208 626 181 615T143 592T132 580H135Q138 579 143 578T153 573T165 566T175 555T183 540T186 520Q186 498 172 481T127 463Z">
            </path>
          </defs>
          <g stroke="currentColor" fill="currentColor" stroke-width="0" transform="matrix(1 0 0 -1 0 0)">
            <use xlink:href="#E18-MJMAIN-2265" x="0" y="0"></use>
            <use xlink:href="#E18-MJMAIN-31" x="1055" y="0"></use>
            <use xlink:href="#E18-MJMAIN-2F" x="1555" y="0"></use>
            <use xlink:href="#E18-MJMAIN-33" x="2055" y="0"></use>
          </g>
        </svg></span>
      <script type="math/tex">{≥1/3}</script> 。</p>
    <p>证明：</p>
    <p>
      考虑一条线段被切分后的所有线段共<strong>n</strong>条，将他们按照长度由大到小依次排列，并且记排列后的数列为<strong>a</strong>。显然，如果一条线段中没有三条线段可以构成三角形，那么他一定满足如下规律
    </p>
    <p><strong><span class="MathJax_SVG" tabindex="-1" style="font-size: 100%; display: inline-block;"><svg
            xmlns:xlink="http://www.w3.org/1999/xlink" width="28.635ex" height="2.308ex"
            viewBox="0 -731.2 12328.8 993.6" role="img" focusable="false" style="vertical-align: -0.609ex;">
            <defs>
              <path stroke-width="0" id="E6-MJMATHI-61"
                d="M33 157Q33 258 109 349T280 441Q331 441 370 392Q386 422 416 422Q429 422 439 414T449 394Q449 381 412 234T374 68Q374 43 381 35T402 26Q411 27 422 35Q443 55 463 131Q469 151 473 152Q475 153 483 153H487Q506 153 506 144Q506 138 501 117T481 63T449 13Q436 0 417 -8Q409 -10 393 -10Q359 -10 336 5T306 36L300 51Q299 52 296 50Q294 48 292 46Q233 -10 172 -10Q117 -10 75 30T33 157ZM351 328Q351 334 346 350T323 385T277 405Q242 405 210 374T160 293Q131 214 119 129Q119 126 119 118T118 106Q118 61 136 44T179 26Q217 26 254 59T298 110Q300 114 325 217T351 328Z">
              </path>
              <path stroke-width="0" id="E6-MJMATHI-69"
                d="M184 600Q184 624 203 642T247 661Q265 661 277 649T290 619Q290 596 270 577T226 557Q211 557 198 567T184 600ZM21 287Q21 295 30 318T54 369T98 420T158 442Q197 442 223 419T250 357Q250 340 236 301T196 196T154 83Q149 61 149 51Q149 26 166 26Q175 26 185 29T208 43T235 78T260 137Q263 149 265 151T282 153Q302 153 302 143Q302 135 293 112T268 61T223 11T161 -11Q129 -11 102 10T74 74Q74 91 79 106T122 220Q160 321 166 341T173 380Q173 404 156 404H154Q124 404 99 371T61 287Q60 286 59 284T58 281T56 279T53 278T49 278T41 278H27Q21 284 21 287Z">
              </path>
              <path stroke-width="0" id="E6-MJMAIN-2B"
                d="M56 237T56 250T70 270H369V420L370 570Q380 583 389 583Q402 583 409 568V270H707Q722 262 722 250T707 230H409V-68Q401 -82 391 -82H389H387Q375 -82 369 -68V230H70Q56 237 56 250Z">
              </path>
              <path stroke-width="0" id="E6-MJMAIN-32"
                d="M109 429Q82 429 66 447T50 491Q50 562 103 614T235 666Q326 666 387 610T449 465Q449 422 429 383T381 315T301 241Q265 210 201 149L142 93L218 92Q375 92 385 97Q392 99 409 186V189H449V186Q448 183 436 95T421 3V0H50V19V31Q50 38 56 46T86 81Q115 113 136 137Q145 147 170 174T204 211T233 244T261 278T284 308T305 340T320 369T333 401T340 431T343 464Q343 527 309 573T212 619Q179 619 154 602T119 569T109 550Q109 549 114 549Q132 549 151 535T170 489Q170 464 154 447T109 429Z">
              </path>
              <path stroke-width="0" id="E6-MJMAIN-2265"
                d="M83 616Q83 624 89 630T99 636Q107 636 253 568T543 431T687 361Q694 356 694 346T687 331Q685 329 395 192L107 56H101Q83 58 83 76Q83 77 83 79Q82 86 98 95Q117 105 248 167Q326 204 378 228L626 346L360 472Q291 505 200 548Q112 589 98 597T83 616ZM84 -118Q84 -108 99 -98H678Q694 -104 694 -118Q694 -130 679 -138H98Q84 -131 84 -118Z">
              </path>
              <path stroke-width="0" id="E6-MJMAIN-31"
                d="M213 578L200 573Q186 568 160 563T102 556H83V602H102Q149 604 189 617T245 641T273 663Q275 666 285 666Q294 666 302 660V361L303 61Q310 54 315 52T339 48T401 46H427V0H416Q395 3 257 3Q121 3 100 0H88V46H114Q136 46 152 46T177 47T193 50T201 52T207 57T213 61V578Z">
              </path>
              <path stroke-width="0" id="E6-MJMAIN-2C"
                d="M78 35T78 60T94 103T137 121Q165 121 187 96T210 8Q210 -27 201 -60T180 -117T154 -158T130 -185T117 -194Q113 -194 104 -185T95 -172Q95 -168 106 -156T131 -126T157 -76T173 -3V9L172 8Q170 7 167 6T161 3T152 1T140 0Q113 0 96 17Z">
              </path>
              <path stroke-width="0" id="E6-MJMAIN-3D"
                d="M56 347Q56 360 70 367H707Q722 359 722 347Q722 336 708 328L390 327H72Q56 332 56 347ZM56 153Q56 168 72 173H708Q722 163 722 153Q722 140 707 133H70Q56 140 56 153Z">
              </path>
              <path stroke-width="0" id="E6-MJMAIN-33"
                d="M127 463Q100 463 85 480T69 524Q69 579 117 622T233 665Q268 665 277 664Q351 652 390 611T430 522Q430 470 396 421T302 350L299 348Q299 347 308 345T337 336T375 315Q457 262 457 175Q457 96 395 37T238 -22Q158 -22 100 21T42 130Q42 158 60 175T105 193Q133 193 151 175T169 130Q169 119 166 110T159 94T148 82T136 74T126 70T118 67L114 66Q165 21 238 21Q293 21 321 74Q338 107 338 175V195Q338 290 274 322Q259 328 213 329L171 330L168 332Q166 335 166 348Q166 366 174 366Q202 366 232 371Q266 376 294 413T322 525V533Q322 590 287 612Q265 626 240 626Q208 626 181 615T143 592T132 580H135Q138 579 143 578T153 573T165 566T175 555T183 540T186 520Q186 498 172 481T127 463Z">
              </path>
              <path stroke-width="0" id="E6-MJMAIN-2E"
                d="M78 60Q78 84 95 102T138 120Q162 120 180 104T199 61Q199 36 182 18T139 0T96 17T78 60Z"></path>
            </defs>
            <g stroke="currentColor" fill="currentColor" stroke-width="0" transform="matrix(1 0 0 -1 0 0)">
              <use xlink:href="#E6-MJMATHI-61" x="0" y="0"></use>
              <g transform="translate(529,-150)">
                <use transform="scale(0.707)" xlink:href="#E6-MJMATHI-69" x="0" y="0"></use>
                <use transform="scale(0.707)" xlink:href="#E6-MJMAIN-2B" x="345" y="0"></use>
                <use transform="scale(0.707)" xlink:href="#E6-MJMAIN-32" x="1123" y="0"></use>
              </g>
              <use xlink:href="#E6-MJMAIN-2265" x="2054" y="0"></use>
              <g transform="translate(3110,0)">
                <use xlink:href="#E6-MJMATHI-61" x="0" y="0"></use>
                <use transform="scale(0.707)" xlink:href="#E6-MJMATHI-69" x="748" y="-213"></use>
              </g>
              <use xlink:href="#E6-MJMAIN-2B" x="4205" y="0"></use>
              <g transform="translate(5205,0)">
                <use xlink:href="#E6-MJMATHI-61" x="0" y="0"></use>
                <g transform="translate(529,-150)">
                  <use transform="scale(0.707)" xlink:href="#E6-MJMATHI-69" x="0" y="0"></use>
                  <use transform="scale(0.707)" xlink:href="#E6-MJMAIN-2B" x="345" y="0"></use>
                  <use transform="scale(0.707)" xlink:href="#E6-MJMAIN-31" x="1123" y="0"></use>
                </g>
              </g>
              <use xlink:href="#E6-MJMAIN-2C" x="6982" y="0"></use>
              <use xlink:href="#E6-MJMATHI-69" x="7426" y="0"></use>
              <use xlink:href="#E6-MJMAIN-3D" x="8049" y="0"></use>
              <use xlink:href="#E6-MJMAIN-31" x="9105" y="0"></use>
              <use xlink:href="#E6-MJMAIN-2C" x="9605" y="0"></use>
              <use xlink:href="#E6-MJMAIN-32" x="10050" y="0"></use>
              <use xlink:href="#E6-MJMAIN-2C" x="10550" y="0"></use>
              <g transform="translate(10994,0)">
                <use xlink:href="#E6-MJMAIN-33"></use>
                <use xlink:href="#E6-MJMAIN-2E" x="500" y="0"></use>
                <use xlink:href="#E6-MJMAIN-2E" x="778" y="0"></use>
                <use xlink:href="#E6-MJMAIN-2E" x="1056" y="0"></use>
              </g>
            </g>
          </svg></span>
        <script type="math/tex">{a_{i+2}≥a_{i}+a_{i+1},i=1,2,3...}</script></strong></p>
    <p>观察到这一点，我们通过尝试发现，实际上</p>
    <p><span class="MathJax_SVG" tabindex="-1" style="font-size: 100%; display: inline-block;"><svg
          xmlns:xlink="http://www.w3.org/1999/xlink" width="42.942ex" height="3.275ex" viewBox="0 -939.5 18488.8 1410.2"
          role="img" focusable="false" style="vertical-align: -1.093ex;">
          <defs>
            <path stroke-width="0" id="E7-MJMATHI-61"
              d="M33 157Q33 258 109 349T280 441Q331 441 370 392Q386 422 416 422Q429 422 439 414T449 394Q449 381 412 234T374 68Q374 43 381 35T402 26Q411 27 422 35Q443 55 463 131Q469 151 473 152Q475 153 483 153H487Q506 153 506 144Q506 138 501 117T481 63T449 13Q436 0 417 -8Q409 -10 393 -10Q359 -10 336 5T306 36L300 51Q299 52 296 50Q294 48 292 46Q233 -10 172 -10Q117 -10 75 30T33 157ZM351 328Q351 334 346 350T323 385T277 405Q242 405 210 374T160 293Q131 214 119 129Q119 126 119 118T118 106Q118 61 136 44T179 26Q217 26 254 59T298 110Q300 114 325 217T351 328Z">
            </path>
            <path stroke-width="0" id="E7-MJMATHI-6E"
              d="M21 287Q22 293 24 303T36 341T56 388T89 425T135 442Q171 442 195 424T225 390T231 369Q231 367 232 367L243 378Q304 442 382 442Q436 442 469 415T503 336T465 179T427 52Q427 26 444 26Q450 26 453 27Q482 32 505 65T540 145Q542 153 560 153Q580 153 580 145Q580 144 576 130Q568 101 554 73T508 17T439 -10Q392 -10 371 17T350 73Q350 92 386 193T423 345Q423 404 379 404H374Q288 404 229 303L222 291L189 157Q156 26 151 16Q138 -11 108 -11Q95 -11 87 -5T76 7T74 17Q74 30 112 180T152 343Q153 348 153 366Q153 405 129 405Q91 405 66 305Q60 285 60 284Q58 278 41 278H27Q21 284 21 287Z">
            </path>
            <path stroke-width="0" id="E7-MJMAIN-2265"
              d="M83 616Q83 624 89 630T99 636Q107 636 253 568T543 431T687 361Q694 356 694 346T687 331Q685 329 395 192L107 56H101Q83 58 83 76Q83 77 83 79Q82 86 98 95Q117 105 248 167Q326 204 378 228L626 346L360 472Q291 505 200 548Q112 589 98 597T83 616ZM84 -118Q84 -108 99 -98H678Q694 -104 694 -118Q694 -130 679 -138H98Q84 -131 84 -118Z">
            </path>
            <path stroke-width="0" id="E7-MJMAIN-31"
              d="M213 578L200 573Q186 568 160 563T102 556H83V602H102Q149 604 189 617T245 641T273 663Q275 666 285 666Q294 666 302 660V361L303 61Q310 54 315 52T339 48T401 46H427V0H416Q395 3 257 3Q121 3 100 0H88V46H114Q136 46 152 46T177 47T193 50T201 52T207 57T213 61V578Z">
            </path>
            <path stroke-width="0" id="E7-MJMAIN-32"
              d="M109 429Q82 429 66 447T50 491Q50 562 103 614T235 666Q326 666 387 610T449 465Q449 422 429 383T381 315T301 241Q265 210 201 149L142 93L218 92Q375 92 385 97Q392 99 409 186V189H449V186Q448 183 436 95T421 3V0H50V19V31Q50 38 56 46T86 81Q115 113 136 137Q145 147 170 174T204 211T233 244T261 278T284 308T305 340T320 369T333 401T340 431T343 464Q343 527 309 573T212 619Q179 619 154 602T119 569T109 550Q109 549 114 549Q132 549 151 535T170 489Q170 464 154 447T109 429Z">
            </path>
            <path stroke-width="0" id="E7-MJMAIN-28"
              d="M94 250Q94 319 104 381T127 488T164 576T202 643T244 695T277 729T302 750H315H319Q333 750 333 741Q333 738 316 720T275 667T226 581T184 443T167 250T184 58T225 -81T274 -167T316 -220T333 -241Q333 -250 318 -250H315H302L274 -226Q180 -141 137 -14T94 250Z">
            </path>
            <path stroke-width="0" id="E7-MJMAIN-2B"
              d="M56 237T56 250T70 270H369V420L370 570Q380 583 389 583Q402 583 409 568V270H707Q722 262 722 250T707 230H409V-68Q401 -82 391 -82H389H387Q375 -82 369 -68V230H70Q56 237 56 250Z">
            </path>
            <path stroke-width="0" id="E7-MJMAIN-2E"
              d="M78 60Q78 84 95 102T138 120Q162 120 180 104T199 61Q199 36 182 18T139 0T96 17T78 60Z"></path>
            <path stroke-width="0" id="E7-MJMAIN-2212"
              d="M84 237T84 250T98 270H679Q694 262 694 250T679 230H98Q84 237 84 250Z"></path>
            <path stroke-width="0" id="E7-MJMAIN-29"
              d="M60 749L64 750Q69 750 74 750H86L114 726Q208 641 251 514T294 250Q294 182 284 119T261 12T224 -76T186 -143T145 -194T113 -227T90 -246Q87 -249 86 -250H74Q66 -250 63 -250T58 -247T55 -238Q56 -237 66 -225Q221 -64 221 250T66 725Q56 737 55 738Q55 746 60 749Z">
            </path>
            <path stroke-width="0" id="E7-MJMAIN-2C"
              d="M78 35T78 60T94 103T137 121Q165 121 187 96T210 8Q210 -27 201 -60T180 -117T154 -158T130 -185T117 -194Q113 -194 104 -185T95 -172Q95 -168 106 -156T131 -126T157 -76T173 -3V9L172 8Q170 7 167 6T161 3T152 1T140 0Q113 0 96 17Z">
            </path>
            <path stroke-width="0" id="E7-MJMAIN-3D"
              d="M56 347Q56 360 70 367H707Q722 359 722 347Q722 336 708 328L390 327H72Q56 332 56 347ZM56 153Q56 168 72 173H708Q722 163 722 153Q722 140 707 133H70Q56 140 56 153Z">
            </path>
            <path stroke-width="0" id="E7-MJMAIN-33"
              d="M127 463Q100 463 85 480T69 524Q69 579 117 622T233 665Q268 665 277 664Q351 652 390 611T430 522Q430 470 396 421T302 350L299 348Q299 347 308 345T337 336T375 315Q457 262 457 175Q457 96 395 37T238 -22Q158 -22 100 21T42 130Q42 158 60 175T105 193Q133 193 151 175T169 130Q169 119 166 110T159 94T148 82T136 74T126 70T118 67L114 66Q165 21 238 21Q293 21 321 74Q338 107 338 175V195Q338 290 274 322Q259 328 213 329L171 330L168 332Q166 335 166 348Q166 366 174 366Q202 366 232 371Q266 376 294 413T322 525V533Q322 590 287 612Q265 626 240 626Q208 626 181 615T143 592T132 580H135Q138 579 143 578T153 573T165 566T175 555T183 540T186 520Q186 498 172 481T127 463Z">
            </path>
          </defs>
          <g stroke="currentColor" fill="currentColor" stroke-width="0" transform="matrix(1 0 0 -1 0 0)">
            <use xlink:href="#E7-MJMATHI-61" x="0" y="0"></use>
            <use transform="scale(0.707)" xlink:href="#E7-MJMATHI-6E" x="748" y="-213"></use>
            <use xlink:href="#E7-MJMAIN-2265" x="1331" y="0"></use>
            <g transform="translate(2109,0)">
              <g transform="translate(397,0)">
                <rect stroke="none" width="473" height="60" x="0" y="220"></rect>
                <use transform="scale(0.707)" xlink:href="#E7-MJMAIN-31" x="84" y="576"></use>
                <use transform="scale(0.707)" xlink:href="#E7-MJMAIN-32" x="84" y="-536"></use>
              </g>
            </g>
            <use xlink:href="#E7-MJMAIN-28" x="3100" y="0"></use>
            <g transform="translate(3489,0)">
              <use xlink:href="#E7-MJMATHI-61" x="0" y="0"></use>
              <use transform="scale(0.707)" xlink:href="#E7-MJMAIN-31" x="748" y="-213"></use>
            </g>
            <use xlink:href="#E7-MJMAIN-2B" x="4471" y="0"></use>
            <use xlink:href="#E7-MJMAIN-2E" x="5249" y="0"></use>
            <use xlink:href="#E7-MJMAIN-2E" x="5694" y="0"></use>
            <use xlink:href="#E7-MJMAIN-2E" x="6139" y="0"></use>
            <use xlink:href="#E7-MJMAIN-2B" x="6583" y="0"></use>
            <g transform="translate(7361,0)">
              <use xlink:href="#E7-MJMATHI-61" x="0" y="0"></use>
              <g transform="translate(529,-150)">
                <use transform="scale(0.707)" xlink:href="#E7-MJMATHI-6E" x="0" y="0"></use>
                <use transform="scale(0.707)" xlink:href="#E7-MJMAIN-2212" x="600" y="0"></use>
                <use transform="scale(0.707)" xlink:href="#E7-MJMAIN-32" x="1378" y="0"></use>
              </g>
            </g>
            <use xlink:href="#E7-MJMAIN-2B" x="9541" y="0"></use>
            <g transform="translate(10541,0)">
              <use xlink:href="#E7-MJMATHI-61" x="0" y="0"></use>
              <g transform="translate(529,-150)">
                <use transform="scale(0.707)" xlink:href="#E7-MJMATHI-6E" x="0" y="0"></use>
                <use transform="scale(0.707)" xlink:href="#E7-MJMAIN-2212" x="600" y="0"></use>
                <use transform="scale(0.707)" xlink:href="#E7-MJMAIN-31" x="1378" y="0"></use>
              </g>
            </g>
            <use xlink:href="#E7-MJMAIN-29" x="12498" y="0"></use>
            <use xlink:href="#E7-MJMAIN-2C" x="12887" y="0"></use>
            <use xlink:href="#E7-MJMATHI-6E" x="13331" y="0"></use>
            <use xlink:href="#E7-MJMAIN-3D" x="14209" y="0"></use>
            <use xlink:href="#E7-MJMAIN-31" x="15265" y="0"></use>
            <use xlink:href="#E7-MJMAIN-2C" x="15765" y="0"></use>
            <use xlink:href="#E7-MJMAIN-32" x="16210" y="0"></use>
            <use xlink:href="#E7-MJMAIN-2C" x="16710" y="0"></use>
            <g transform="translate(17154,0)">
              <use xlink:href="#E7-MJMAIN-33"></use>
              <use xlink:href="#E7-MJMAIN-2E" x="500" y="0"></use>
              <use xlink:href="#E7-MJMAIN-2E" x="778" y="0"></use>
              <use xlink:href="#E7-MJMAIN-2E" x="1056" y="0"></use>
            </g>
          </g>
        </svg></span>
      <script type="math/tex">{a_{n}≥\frac{1}{2}(a_1+...+a_{n-2}+a_{n-1}),n=1,2,3...}</script> (1)</p>
    <p>显然，(1) 对 n=1,2,3均成立。假设(1)对于任何<span class="MathJax_SVG" tabindex="-1"
        style="font-size: 100%; display: inline-block;"><svg xmlns:xlink="http://www.w3.org/1999/xlink" width="5.469ex"
          height="2.308ex" viewBox="0 -783.2 2354.6 993.6" role="img" focusable="false"
          style="vertical-align: -0.489ex;">
          <defs>
            <path stroke-width="0" id="E8-MJMATHI-6B"
              d="M121 647Q121 657 125 670T137 683Q138 683 209 688T282 694Q294 694 294 686Q294 679 244 477Q194 279 194 272Q213 282 223 291Q247 309 292 354T362 415Q402 442 438 442Q468 442 485 423T503 369Q503 344 496 327T477 302T456 291T438 288Q418 288 406 299T394 328Q394 353 410 369T442 390L458 393Q446 405 434 405H430Q398 402 367 380T294 316T228 255Q230 254 243 252T267 246T293 238T320 224T342 206T359 180T365 147Q365 130 360 106T354 66Q354 26 381 26Q429 26 459 145Q461 153 479 153H483Q499 153 499 144Q499 139 496 130Q455 -11 378 -11Q333 -11 305 15T277 90Q277 108 280 121T283 145Q283 167 269 183T234 206T200 217T182 220H180Q168 178 159 139T145 81T136 44T129 20T122 7T111 -2Q98 -11 83 -11Q66 -11 57 -1T48 16Q48 26 85 176T158 471L195 616Q196 629 188 632T149 637H144Q134 637 131 637T124 640T121 647Z">
            </path>
            <path stroke-width="0" id="E8-MJMAIN-2265"
              d="M83 616Q83 624 89 630T99 636Q107 636 253 568T543 431T687 361Q694 356 694 346T687 331Q685 329 395 192L107 56H101Q83 58 83 76Q83 77 83 79Q82 86 98 95Q117 105 248 167Q326 204 378 228L626 346L360 472Q291 505 200 548Q112 589 98 597T83 616ZM84 -118Q84 -108 99 -98H678Q694 -104 694 -118Q694 -130 679 -138H98Q84 -131 84 -118Z">
            </path>
            <path stroke-width="0" id="E8-MJMAIN-33"
              d="M127 463Q100 463 85 480T69 524Q69 579 117 622T233 665Q268 665 277 664Q351 652 390 611T430 522Q430 470 396 421T302 350L299 348Q299 347 308 345T337 336T375 315Q457 262 457 175Q457 96 395 37T238 -22Q158 -22 100 21T42 130Q42 158 60 175T105 193Q133 193 151 175T169 130Q169 119 166 110T159 94T148 82T136 74T126 70T118 67L114 66Q165 21 238 21Q293 21 321 74Q338 107 338 175V195Q338 290 274 322Q259 328 213 329L171 330L168 332Q166 335 166 348Q166 366 174 366Q202 366 232 371Q266 376 294 413T322 525V533Q322 590 287 612Q265 626 240 626Q208 626 181 615T143 592T132 580H135Q138 579 143 578T153 573T165 566T175 555T183 540T186 520Q186 498 172 481T127 463Z">
            </path>
          </defs>
          <g stroke="currentColor" fill="currentColor" stroke-width="0" transform="matrix(1 0 0 -1 0 0)">
            <use xlink:href="#E8-MJMATHI-6B" x="0" y="0"></use>
            <use xlink:href="#E8-MJMAIN-2265" x="798" y="0"></use>
            <use xlink:href="#E8-MJMAIN-33" x="1854" y="0"></use>
          </g>
        </svg></span>
      <script type="math/tex">{k≥3}</script> 均成立，考虑<span class="MathJax_SVG" tabindex="-1"
        style="font-size: 100%; display: inline-block;"><svg xmlns:xlink="http://www.w3.org/1999/xlink" width="5.211ex"
          height="2.187ex" viewBox="0 -783.2 2243.4 941.5" role="img" focusable="false"
          style="vertical-align: -0.368ex;">
          <defs>
            <path stroke-width="0" id="E9-MJMATHI-6B"
              d="M121 647Q121 657 125 670T137 683Q138 683 209 688T282 694Q294 694 294 686Q294 679 244 477Q194 279 194 272Q213 282 223 291Q247 309 292 354T362 415Q402 442 438 442Q468 442 485 423T503 369Q503 344 496 327T477 302T456 291T438 288Q418 288 406 299T394 328Q394 353 410 369T442 390L458 393Q446 405 434 405H430Q398 402 367 380T294 316T228 255Q230 254 243 252T267 246T293 238T320 224T342 206T359 180T365 147Q365 130 360 106T354 66Q354 26 381 26Q429 26 459 145Q461 153 479 153H483Q499 153 499 144Q499 139 496 130Q455 -11 378 -11Q333 -11 305 15T277 90Q277 108 280 121T283 145Q283 167 269 183T234 206T200 217T182 220H180Q168 178 159 139T145 81T136 44T129 20T122 7T111 -2Q98 -11 83 -11Q66 -11 57 -1T48 16Q48 26 85 176T158 471L195 616Q196 629 188 632T149 637H144Q134 637 131 637T124 640T121 647Z">
            </path>
            <path stroke-width="0" id="E9-MJMAIN-2B"
              d="M56 237T56 250T70 270H369V420L370 570Q380 583 389 583Q402 583 409 568V270H707Q722 262 722 250T707 230H409V-68Q401 -82 391 -82H389H387Q375 -82 369 -68V230H70Q56 237 56 250Z">
            </path>
            <path stroke-width="0" id="E9-MJMAIN-31"
              d="M213 578L200 573Q186 568 160 563T102 556H83V602H102Q149 604 189 617T245 641T273 663Q275 666 285 666Q294 666 302 660V361L303 61Q310 54 315 52T339 48T401 46H427V0H416Q395 3 257 3Q121 3 100 0H88V46H114Q136 46 152 46T177 47T193 50T201 52T207 57T213 61V578Z">
            </path>
          </defs>
          <g stroke="currentColor" fill="currentColor" stroke-width="0" transform="matrix(1 0 0 -1 0 0)">
            <use xlink:href="#E9-MJMATHI-6B" x="0" y="0"></use>
            <use xlink:href="#E9-MJMAIN-2B" x="743" y="0"></use>
            <use xlink:href="#E9-MJMAIN-31" x="1743" y="0"></use>
          </g>
        </svg></span>
      <script type="math/tex">{k+1}</script>的情况，观察一下已知情况</p>
    <ol start=''>
      <li><span class="MathJax_SVG" tabindex="-1" style="font-size: 100%; display: inline-block;"><svg
            xmlns:xlink="http://www.w3.org/1999/xlink" width="17.473ex" height="2.308ex" viewBox="0 -731.2 7523.2 993.6"
            role="img" focusable="false" style="vertical-align: -0.609ex;">
            <defs>
              <path stroke-width="0" id="E10-MJMATHI-61"
                d="M33 157Q33 258 109 349T280 441Q331 441 370 392Q386 422 416 422Q429 422 439 414T449 394Q449 381 412 234T374 68Q374 43 381 35T402 26Q411 27 422 35Q443 55 463 131Q469 151 473 152Q475 153 483 153H487Q506 153 506 144Q506 138 501 117T481 63T449 13Q436 0 417 -8Q409 -10 393 -10Q359 -10 336 5T306 36L300 51Q299 52 296 50Q294 48 292 46Q233 -10 172 -10Q117 -10 75 30T33 157ZM351 328Q351 334 346 350T323 385T277 405Q242 405 210 374T160 293Q131 214 119 129Q119 126 119 118T118 106Q118 61 136 44T179 26Q217 26 254 59T298 110Q300 114 325 217T351 328Z">
              </path>
              <path stroke-width="0" id="E10-MJMATHI-6E"
                d="M21 287Q22 293 24 303T36 341T56 388T89 425T135 442Q171 442 195 424T225 390T231 369Q231 367 232 367L243 378Q304 442 382 442Q436 442 469 415T503 336T465 179T427 52Q427 26 444 26Q450 26 453 27Q482 32 505 65T540 145Q542 153 560 153Q580 153 580 145Q580 144 576 130Q568 101 554 73T508 17T439 -10Q392 -10 371 17T350 73Q350 92 386 193T423 345Q423 404 379 404H374Q288 404 229 303L222 291L189 157Q156 26 151 16Q138 -11 108 -11Q95 -11 87 -5T76 7T74 17Q74 30 112 180T152 343Q153 348 153 366Q153 405 129 405Q91 405 66 305Q60 285 60 284Q58 278 41 278H27Q21 284 21 287Z">
              </path>
              <path stroke-width="0" id="E10-MJMAIN-2B"
                d="M56 237T56 250T70 270H369V420L370 570Q380 583 389 583Q402 583 409 568V270H707Q722 262 722 250T707 230H409V-68Q401 -82 391 -82H389H387Q375 -82 369 -68V230H70Q56 237 56 250Z">
              </path>
              <path stroke-width="0" id="E10-MJMAIN-31"
                d="M213 578L200 573Q186 568 160 563T102 556H83V602H102Q149 604 189 617T245 641T273 663Q275 666 285 666Q294 666 302 660V361L303 61Q310 54 315 52T339 48T401 46H427V0H416Q395 3 257 3Q121 3 100 0H88V46H114Q136 46 152 46T177 47T193 50T201 52T207 57T213 61V578Z">
              </path>
              <path stroke-width="0" id="E10-MJMAIN-2265"
                d="M83 616Q83 624 89 630T99 636Q107 636 253 568T543 431T687 361Q694 356 694 346T687 331Q685 329 395 192L107 56H101Q83 58 83 76Q83 77 83 79Q82 86 98 95Q117 105 248 167Q326 204 378 228L626 346L360 472Q291 505 200 548Q112 589 98 597T83 616ZM84 -118Q84 -108 99 -98H678Q694 -104 694 -118Q694 -130 679 -138H98Q84 -131 84 -118Z">
              </path>
              <path stroke-width="0" id="E10-MJMAIN-2212"
                d="M84 237T84 250T98 270H679Q694 262 694 250T679 230H98Q84 237 84 250Z"></path>
            </defs>
            <g stroke="currentColor" fill="currentColor" stroke-width="0" transform="matrix(1 0 0 -1 0 0)">
              <use xlink:href="#E10-MJMATHI-61" x="0" y="0"></use>
              <g transform="translate(529,-150)">
                <use transform="scale(0.707)" xlink:href="#E10-MJMATHI-6E" x="0" y="0"></use>
                <use transform="scale(0.707)" xlink:href="#E10-MJMAIN-2B" x="600" y="0"></use>
                <use transform="scale(0.707)" xlink:href="#E10-MJMAIN-31" x="1378" y="0"></use>
              </g>
              <use xlink:href="#E10-MJMAIN-2265" x="2234" y="0"></use>
              <g transform="translate(3290,0)">
                <use xlink:href="#E10-MJMATHI-61" x="0" y="0"></use>
                <use transform="scale(0.707)" xlink:href="#E10-MJMATHI-6E" x="748" y="-213"></use>
              </g>
              <use xlink:href="#E10-MJMAIN-2B" x="4565" y="0"></use>
              <g transform="translate(5566,0)">
                <use xlink:href="#E10-MJMATHI-61" x="0" y="0"></use>
                <g transform="translate(529,-150)">
                  <use transform="scale(0.707)" xlink:href="#E10-MJMATHI-6E" x="0" y="0"></use>
                  <use transform="scale(0.707)" xlink:href="#E10-MJMAIN-2212" x="600" y="0"></use>
                  <use transform="scale(0.707)" xlink:href="#E10-MJMAIN-31" x="1378" y="0"></use>
                </g>
              </g>
            </g>
          </svg></span>
        <script type="math/tex">{a_{n+1}≥a_{n}+a_{n-1}}</script>
      </li>
      <li><span class="MathJax_SVG" tabindex="-1" style="font-size: 100%; display: inline-block;"><svg
            xmlns:xlink="http://www.w3.org/1999/xlink" width="17.731ex" height="2.308ex" viewBox="0 -731.2 7634.3 993.6"
            role="img" focusable="false" style="vertical-align: -0.609ex;">
            <defs>
              <path stroke-width="0" id="E11-MJMATHI-61"
                d="M33 157Q33 258 109 349T280 441Q331 441 370 392Q386 422 416 422Q429 422 439 414T449 394Q449 381 412 234T374 68Q374 43 381 35T402 26Q411 27 422 35Q443 55 463 131Q469 151 473 152Q475 153 483 153H487Q506 153 506 144Q506 138 501 117T481 63T449 13Q436 0 417 -8Q409 -10 393 -10Q359 -10 336 5T306 36L300 51Q299 52 296 50Q294 48 292 46Q233 -10 172 -10Q117 -10 75 30T33 157ZM351 328Q351 334 346 350T323 385T277 405Q242 405 210 374T160 293Q131 214 119 129Q119 126 119 118T118 106Q118 61 136 44T179 26Q217 26 254 59T298 110Q300 114 325 217T351 328Z">
              </path>
              <path stroke-width="0" id="E11-MJMATHI-6E"
                d="M21 287Q22 293 24 303T36 341T56 388T89 425T135 442Q171 442 195 424T225 390T231 369Q231 367 232 367L243 378Q304 442 382 442Q436 442 469 415T503 336T465 179T427 52Q427 26 444 26Q450 26 453 27Q482 32 505 65T540 145Q542 153 560 153Q580 153 580 145Q580 144 576 130Q568 101 554 73T508 17T439 -10Q392 -10 371 17T350 73Q350 92 386 193T423 345Q423 404 379 404H374Q288 404 229 303L222 291L189 157Q156 26 151 16Q138 -11 108 -11Q95 -11 87 -5T76 7T74 17Q74 30 112 180T152 343Q153 348 153 366Q153 405 129 405Q91 405 66 305Q60 285 60 284Q58 278 41 278H27Q21 284 21 287Z">
              </path>
              <path stroke-width="0" id="E11-MJMAIN-2B"
                d="M56 237T56 250T70 270H369V420L370 570Q380 583 389 583Q402 583 409 568V270H707Q722 262 722 250T707 230H409V-68Q401 -82 391 -82H389H387Q375 -82 369 -68V230H70Q56 237 56 250Z">
              </path>
              <path stroke-width="0" id="E11-MJMAIN-31"
                d="M213 578L200 573Q186 568 160 563T102 556H83V602H102Q149 604 189 617T245 641T273 663Q275 666 285 666Q294 666 302 660V361L303 61Q310 54 315 52T339 48T401 46H427V0H416Q395 3 257 3Q121 3 100 0H88V46H114Q136 46 152 46T177 47T193 50T201 52T207 57T213 61V578Z">
              </path>
              <path stroke-width="0" id="E11-MJMAIN-2265"
                d="M83 616Q83 624 89 630T99 636Q107 636 253 568T543 431T687 361Q694 356 694 346T687 331Q685 329 395 192L107 56H101Q83 58 83 76Q83 77 83 79Q82 86 98 95Q117 105 248 167Q326 204 378 228L626 346L360 472Q291 505 200 548Q112 589 98 597T83 616ZM84 -118Q84 -108 99 -98H678Q694 -104 694 -118Q694 -130 679 -138H98Q84 -131 84 -118Z">
              </path>
              <path stroke-width="0" id="E11-MJMAIN-2212"
                d="M84 237T84 250T98 270H679Q694 262 694 250T679 230H98Q84 237 84 250Z"></path>
            </defs>
            <g stroke="currentColor" fill="currentColor" stroke-width="0" transform="matrix(1 0 0 -1 0 0)">
              <use xlink:href="#E11-MJMATHI-61" x="0" y="0"></use>
              <g transform="translate(529,-150)">
                <use transform="scale(0.707)" xlink:href="#E11-MJMATHI-6E" x="0" y="0"></use>
                <use transform="scale(0.707)" xlink:href="#E11-MJMAIN-2B" x="600" y="0"></use>
                <use transform="scale(0.707)" xlink:href="#E11-MJMAIN-31" x="1378" y="0"></use>
              </g>
              <use xlink:href="#E11-MJMAIN-2265" x="2234" y="0"></use>
              <g transform="translate(3290,0)">
                <use xlink:href="#E11-MJMATHI-61" x="0" y="0"></use>
                <use transform="scale(0.707)" xlink:href="#E11-MJMATHI-6E" x="748" y="-213"></use>
              </g>
              <use xlink:href="#E11-MJMAIN-2265" x="4621" y="0"></use>
              <g transform="translate(5677,0)">
                <use xlink:href="#E11-MJMATHI-61" x="0" y="0"></use>
                <g transform="translate(529,-150)">
                  <use transform="scale(0.707)" xlink:href="#E11-MJMATHI-6E" x="0" y="0"></use>
                  <use transform="scale(0.707)" xlink:href="#E11-MJMAIN-2212" x="600" y="0"></use>
                  <use transform="scale(0.707)" xlink:href="#E11-MJMAIN-31" x="1378" y="0"></use>
                </g>
              </g>
            </g>
          </svg></span>
        <script type="math/tex">{a_{n+1}≥a_{n}≥a_{n-1}}</script>
      </li>
      <li><span class="MathJax_SVG" tabindex="-1" style="font-size: 100%; display: inline-block;"><svg
            xmlns:xlink="http://www.w3.org/1999/xlink" width="27.465ex" height="2.308ex" viewBox="0 -731.2 11825 993.6"
            role="img" focusable="false" style="vertical-align: -0.609ex;">
            <defs>
              <path stroke-width="0" id="E12-MJMAIN-32"
                d="M109 429Q82 429 66 447T50 491Q50 562 103 614T235 666Q326 666 387 610T449 465Q449 422 429 383T381 315T301 241Q265 210 201 149L142 93L218 92Q375 92 385 97Q392 99 409 186V189H449V186Q448 183 436 95T421 3V0H50V19V31Q50 38 56 46T86 81Q115 113 136 137Q145 147 170 174T204 211T233 244T261 278T284 308T305 340T320 369T333 401T340 431T343 464Q343 527 309 573T212 619Q179 619 154 602T119 569T109 550Q109 549 114 549Q132 549 151 535T170 489Q170 464 154 447T109 429Z">
              </path>
              <path stroke-width="0" id="E12-MJMATHI-61"
                d="M33 157Q33 258 109 349T280 441Q331 441 370 392Q386 422 416 422Q429 422 439 414T449 394Q449 381 412 234T374 68Q374 43 381 35T402 26Q411 27 422 35Q443 55 463 131Q469 151 473 152Q475 153 483 153H487Q506 153 506 144Q506 138 501 117T481 63T449 13Q436 0 417 -8Q409 -10 393 -10Q359 -10 336 5T306 36L300 51Q299 52 296 50Q294 48 292 46Q233 -10 172 -10Q117 -10 75 30T33 157ZM351 328Q351 334 346 350T323 385T277 405Q242 405 210 374T160 293Q131 214 119 129Q119 126 119 118T118 106Q118 61 136 44T179 26Q217 26 254 59T298 110Q300 114 325 217T351 328Z">
              </path>
              <path stroke-width="0" id="E12-MJMATHI-6E"
                d="M21 287Q22 293 24 303T36 341T56 388T89 425T135 442Q171 442 195 424T225 390T231 369Q231 367 232 367L243 378Q304 442 382 442Q436 442 469 415T503 336T465 179T427 52Q427 26 444 26Q450 26 453 27Q482 32 505 65T540 145Q542 153 560 153Q580 153 580 145Q580 144 576 130Q568 101 554 73T508 17T439 -10Q392 -10 371 17T350 73Q350 92 386 193T423 345Q423 404 379 404H374Q288 404 229 303L222 291L189 157Q156 26 151 16Q138 -11 108 -11Q95 -11 87 -5T76 7T74 17Q74 30 112 180T152 343Q153 348 153 366Q153 405 129 405Q91 405 66 305Q60 285 60 284Q58 278 41 278H27Q21 284 21 287Z">
              </path>
              <path stroke-width="0" id="E12-MJMAIN-2212"
                d="M84 237T84 250T98 270H679Q694 262 694 250T679 230H98Q84 237 84 250Z"></path>
              <path stroke-width="0" id="E12-MJMAIN-31"
                d="M213 578L200 573Q186 568 160 563T102 556H83V602H102Q149 604 189 617T245 641T273 663Q275 666 285 666Q294 666 302 660V361L303 61Q310 54 315 52T339 48T401 46H427V0H416Q395 3 257 3Q121 3 100 0H88V46H114Q136 46 152 46T177 47T193 50T201 52T207 57T213 61V578Z">
              </path>
              <path stroke-width="0" id="E12-MJMAIN-2265"
                d="M83 616Q83 624 89 630T99 636Q107 636 253 568T543 431T687 361Q694 356 694 346T687 331Q685 329 395 192L107 56H101Q83 58 83 76Q83 77 83 79Q82 86 98 95Q117 105 248 167Q326 204 378 228L626 346L360 472Q291 505 200 548Q112 589 98 597T83 616ZM84 -118Q84 -108 99 -98H678Q694 -104 694 -118Q694 -130 679 -138H98Q84 -131 84 -118Z">
              </path>
              <path stroke-width="0" id="E12-MJMAIN-2B"
                d="M56 237T56 250T70 270H369V420L370 570Q380 583 389 583Q402 583 409 568V270H707Q722 262 722 250T707 230H409V-68Q401 -82 391 -82H389H387Q375 -82 369 -68V230H70Q56 237 56 250Z">
              </path>
              <path stroke-width="0" id="E12-MJMAIN-2E"
                d="M78 60Q78 84 95 102T138 120Q162 120 180 104T199 61Q199 36 182 18T139 0T96 17T78 60Z"></path>
            </defs>
            <g stroke="currentColor" fill="currentColor" stroke-width="0" transform="matrix(1 0 0 -1 0 0)">
              <use xlink:href="#E12-MJMAIN-32" x="0" y="0"></use>
              <g transform="translate(500,0)">
                <use xlink:href="#E12-MJMATHI-61" x="0" y="0"></use>
                <g transform="translate(529,-150)">
                  <use transform="scale(0.707)" xlink:href="#E12-MJMATHI-6E" x="0" y="0"></use>
                  <use transform="scale(0.707)" xlink:href="#E12-MJMAIN-2212" x="600" y="0"></use>
                  <use transform="scale(0.707)" xlink:href="#E12-MJMAIN-31" x="1378" y="0"></use>
                </g>
              </g>
              <use xlink:href="#E12-MJMAIN-2265" x="2734" y="0"></use>
              <g transform="translate(3790,0)">
                <use xlink:href="#E12-MJMATHI-61" x="0" y="0"></use>
                <use transform="scale(0.707)" xlink:href="#E12-MJMAIN-31" x="748" y="-213"></use>
              </g>
              <use xlink:href="#E12-MJMAIN-2B" x="4995" y="0"></use>
              <g transform="translate(5995,0)">
                <use xlink:href="#E12-MJMATHI-61" x="0" y="0"></use>
                <use transform="scale(0.707)" xlink:href="#E12-MJMAIN-32" x="748" y="-213"></use>
              </g>
              <use xlink:href="#E12-MJMAIN-2B" x="6978" y="0"></use>
              <use xlink:href="#E12-MJMAIN-2E" x="7756" y="0"></use>
              <use xlink:href="#E12-MJMAIN-2E" x="8200" y="0"></use>
              <use xlink:href="#E12-MJMAIN-2E" x="8645" y="0"></use>
              <use xlink:href="#E12-MJMAIN-2B" x="9090" y="0"></use>
              <g transform="translate(9868,0)">
                <use xlink:href="#E12-MJMATHI-61" x="0" y="0"></use>
                <g transform="translate(529,-150)">
                  <use transform="scale(0.707)" xlink:href="#E12-MJMATHI-6E" x="0" y="0"></use>
                  <use transform="scale(0.707)" xlink:href="#E12-MJMAIN-2212" x="600" y="0"></use>
                  <use transform="scale(0.707)" xlink:href="#E12-MJMAIN-32" x="1378" y="0"></use>
                </g>
              </g>
            </g>
          </svg></span>
        <script type="math/tex">{2a_{n-1}≥a_1+a_2+...+a_{n-2}}</script>
      </li>

    </ol>
    <p>所以，<span class="MathJax_SVG" tabindex="-1" style="font-size: 100%; display: inline-block;"><svg
          xmlns:xlink="http://www.w3.org/1999/xlink" width="35.107ex" height="2.308ex" viewBox="0 -731.2 15115.5 993.6"
          role="img" focusable="false" style="vertical-align: -0.609ex;">
          <defs>
            <path stroke-width="0" id="E13-MJMATHI-61"
              d="M33 157Q33 258 109 349T280 441Q331 441 370 392Q386 422 416 422Q429 422 439 414T449 394Q449 381 412 234T374 68Q374 43 381 35T402 26Q411 27 422 35Q443 55 463 131Q469 151 473 152Q475 153 483 153H487Q506 153 506 144Q506 138 501 117T481 63T449 13Q436 0 417 -8Q409 -10 393 -10Q359 -10 336 5T306 36L300 51Q299 52 296 50Q294 48 292 46Q233 -10 172 -10Q117 -10 75 30T33 157ZM351 328Q351 334 346 350T323 385T277 405Q242 405 210 374T160 293Q131 214 119 129Q119 126 119 118T118 106Q118 61 136 44T179 26Q217 26 254 59T298 110Q300 114 325 217T351 328Z">
            </path>
            <path stroke-width="0" id="E13-MJMATHI-6E"
              d="M21 287Q22 293 24 303T36 341T56 388T89 425T135 442Q171 442 195 424T225 390T231 369Q231 367 232 367L243 378Q304 442 382 442Q436 442 469 415T503 336T465 179T427 52Q427 26 444 26Q450 26 453 27Q482 32 505 65T540 145Q542 153 560 153Q580 153 580 145Q580 144 576 130Q568 101 554 73T508 17T439 -10Q392 -10 371 17T350 73Q350 92 386 193T423 345Q423 404 379 404H374Q288 404 229 303L222 291L189 157Q156 26 151 16Q138 -11 108 -11Q95 -11 87 -5T76 7T74 17Q74 30 112 180T152 343Q153 348 153 366Q153 405 129 405Q91 405 66 305Q60 285 60 284Q58 278 41 278H27Q21 284 21 287Z">
            </path>
            <path stroke-width="0" id="E13-MJMAIN-2B"
              d="M56 237T56 250T70 270H369V420L370 570Q380 583 389 583Q402 583 409 568V270H707Q722 262 722 250T707 230H409V-68Q401 -82 391 -82H389H387Q375 -82 369 -68V230H70Q56 237 56 250Z">
            </path>
            <path stroke-width="0" id="E13-MJMAIN-31"
              d="M213 578L200 573Q186 568 160 563T102 556H83V602H102Q149 604 189 617T245 641T273 663Q275 666 285 666Q294 666 302 660V361L303 61Q310 54 315 52T339 48T401 46H427V0H416Q395 3 257 3Q121 3 100 0H88V46H114Q136 46 152 46T177 47T193 50T201 52T207 57T213 61V578Z">
            </path>
            <path stroke-width="0" id="E13-MJMAIN-2265"
              d="M83 616Q83 624 89 630T99 636Q107 636 253 568T543 431T687 361Q694 356 694 346T687 331Q685 329 395 192L107 56H101Q83 58 83 76Q83 77 83 79Q82 86 98 95Q117 105 248 167Q326 204 378 228L626 346L360 472Q291 505 200 548Q112 589 98 597T83 616ZM84 -118Q84 -108 99 -98H678Q694 -104 694 -118Q694 -130 679 -138H98Q84 -131 84 -118Z">
            </path>
            <path stroke-width="0" id="E13-MJMAIN-32"
              d="M109 429Q82 429 66 447T50 491Q50 562 103 614T235 666Q326 666 387 610T449 465Q449 422 429 383T381 315T301 241Q265 210 201 149L142 93L218 92Q375 92 385 97Q392 99 409 186V189H449V186Q448 183 436 95T421 3V0H50V19V31Q50 38 56 46T86 81Q115 113 136 137Q145 147 170 174T204 211T233 244T261 278T284 308T305 340T320 369T333 401T340 431T343 464Q343 527 309 573T212 619Q179 619 154 602T119 569T109 550Q109 549 114 549Q132 549 151 535T170 489Q170 464 154 447T109 429Z">
            </path>
            <path stroke-width="0" id="E13-MJMAIN-2212"
              d="M84 237T84 250T98 270H679Q694 262 694 250T679 230H98Q84 237 84 250Z"></path>
            <path stroke-width="0" id="E13-MJMAIN-2E"
              d="M78 60Q78 84 95 102T138 120Q162 120 180 104T199 61Q199 36 182 18T139 0T96 17T78 60Z"></path>
          </defs>
          <g stroke="currentColor" fill="currentColor" stroke-width="0" transform="matrix(1 0 0 -1 0 0)">
            <use xlink:href="#E13-MJMATHI-61" x="0" y="0"></use>
            <g transform="translate(529,-150)">
              <use transform="scale(0.707)" xlink:href="#E13-MJMATHI-6E" x="0" y="0"></use>
              <use transform="scale(0.707)" xlink:href="#E13-MJMAIN-2B" x="600" y="0"></use>
              <use transform="scale(0.707)" xlink:href="#E13-MJMAIN-31" x="1378" y="0"></use>
            </g>
            <use xlink:href="#E13-MJMAIN-2265" x="2234" y="0"></use>
            <use xlink:href="#E13-MJMAIN-32" x="3290" y="0"></use>
            <g transform="translate(3790,0)">
              <use xlink:href="#E13-MJMATHI-61" x="0" y="0"></use>
              <g transform="translate(529,-150)">
                <use transform="scale(0.707)" xlink:href="#E13-MJMATHI-6E" x="0" y="0"></use>
                <use transform="scale(0.707)" xlink:href="#E13-MJMAIN-2212" x="600" y="0"></use>
                <use transform="scale(0.707)" xlink:href="#E13-MJMAIN-31" x="1378" y="0"></use>
              </g>
            </g>
            <use xlink:href="#E13-MJMAIN-2265" x="6025" y="0"></use>
            <g transform="translate(7081,0)">
              <use xlink:href="#E13-MJMATHI-61" x="0" y="0"></use>
              <use transform="scale(0.707)" xlink:href="#E13-MJMAIN-31" x="748" y="-213"></use>
            </g>
            <use xlink:href="#E13-MJMAIN-2B" x="8285" y="0"></use>
            <g transform="translate(9286,0)">
              <use xlink:href="#E13-MJMATHI-61" x="0" y="0"></use>
              <use transform="scale(0.707)" xlink:href="#E13-MJMAIN-32" x="748" y="-213"></use>
            </g>
            <use xlink:href="#E13-MJMAIN-2B" x="10268" y="0"></use>
            <use xlink:href="#E13-MJMAIN-2E" x="11046" y="0"></use>
            <use xlink:href="#E13-MJMAIN-2E" x="11491" y="0"></use>
            <use xlink:href="#E13-MJMAIN-2E" x="11935" y="0"></use>
            <use xlink:href="#E13-MJMAIN-2B" x="12380" y="0"></use>
            <g transform="translate(13158,0)">
              <use xlink:href="#E13-MJMATHI-61" x="0" y="0"></use>
              <g transform="translate(529,-150)">
                <use transform="scale(0.707)" xlink:href="#E13-MJMATHI-6E" x="0" y="0"></use>
                <use transform="scale(0.707)" xlink:href="#E13-MJMAIN-2212" x="600" y="0"></use>
                <use transform="scale(0.707)" xlink:href="#E13-MJMAIN-32" x="1378" y="0"></use>
              </g>
            </g>
          </g>
        </svg></span>
      <script type="math/tex">{a_{n+1}≥2a_{n-1}≥a_1+a_2+...+a_{n-2}}</script>
    </p>
    <p>再结合1. 中的情况，显然有<span class="MathJax_SVG" tabindex="-1" style="font-size: 100%; display: inline-block;"><svg
          xmlns:xlink="http://www.w3.org/1999/xlink" width="42.438ex" height="3.275ex" viewBox="0 -939.5 18271.7 1410.2"
          role="img" focusable="false" style="vertical-align: -1.093ex;">
          <defs>
            <path stroke-width="0" id="E14-MJMATHI-61"
              d="M33 157Q33 258 109 349T280 441Q331 441 370 392Q386 422 416 422Q429 422 439 414T449 394Q449 381 412 234T374 68Q374 43 381 35T402 26Q411 27 422 35Q443 55 463 131Q469 151 473 152Q475 153 483 153H487Q506 153 506 144Q506 138 501 117T481 63T449 13Q436 0 417 -8Q409 -10 393 -10Q359 -10 336 5T306 36L300 51Q299 52 296 50Q294 48 292 46Q233 -10 172 -10Q117 -10 75 30T33 157ZM351 328Q351 334 346 350T323 385T277 405Q242 405 210 374T160 293Q131 214 119 129Q119 126 119 118T118 106Q118 61 136 44T179 26Q217 26 254 59T298 110Q300 114 325 217T351 328Z">
            </path>
            <path stroke-width="0" id="E14-MJMATHI-6E"
              d="M21 287Q22 293 24 303T36 341T56 388T89 425T135 442Q171 442 195 424T225 390T231 369Q231 367 232 367L243 378Q304 442 382 442Q436 442 469 415T503 336T465 179T427 52Q427 26 444 26Q450 26 453 27Q482 32 505 65T540 145Q542 153 560 153Q580 153 580 145Q580 144 576 130Q568 101 554 73T508 17T439 -10Q392 -10 371 17T350 73Q350 92 386 193T423 345Q423 404 379 404H374Q288 404 229 303L222 291L189 157Q156 26 151 16Q138 -11 108 -11Q95 -11 87 -5T76 7T74 17Q74 30 112 180T152 343Q153 348 153 366Q153 405 129 405Q91 405 66 305Q60 285 60 284Q58 278 41 278H27Q21 284 21 287Z">
            </path>
            <path stroke-width="0" id="E14-MJMAIN-2B"
              d="M56 237T56 250T70 270H369V420L370 570Q380 583 389 583Q402 583 409 568V270H707Q722 262 722 250T707 230H409V-68Q401 -82 391 -82H389H387Q375 -82 369 -68V230H70Q56 237 56 250Z">
            </path>
            <path stroke-width="0" id="E14-MJMAIN-31"
              d="M213 578L200 573Q186 568 160 563T102 556H83V602H102Q149 604 189 617T245 641T273 663Q275 666 285 666Q294 666 302 660V361L303 61Q310 54 315 52T339 48T401 46H427V0H416Q395 3 257 3Q121 3 100 0H88V46H114Q136 46 152 46T177 47T193 50T201 52T207 57T213 61V578Z">
            </path>
            <path stroke-width="0" id="E14-MJMAIN-2265"
              d="M83 616Q83 624 89 630T99 636Q107 636 253 568T543 431T687 361Q694 356 694 346T687 331Q685 329 395 192L107 56H101Q83 58 83 76Q83 77 83 79Q82 86 98 95Q117 105 248 167Q326 204 378 228L626 346L360 472Q291 505 200 548Q112 589 98 597T83 616ZM84 -118Q84 -108 99 -98H678Q694 -104 694 -118Q694 -130 679 -138H98Q84 -131 84 -118Z">
            </path>
            <path stroke-width="0" id="E14-MJMAIN-32"
              d="M109 429Q82 429 66 447T50 491Q50 562 103 614T235 666Q326 666 387 610T449 465Q449 422 429 383T381 315T301 241Q265 210 201 149L142 93L218 92Q375 92 385 97Q392 99 409 186V189H449V186Q448 183 436 95T421 3V0H50V19V31Q50 38 56 46T86 81Q115 113 136 137Q145 147 170 174T204 211T233 244T261 278T284 308T305 340T320 369T333 401T340 431T343 464Q343 527 309 573T212 619Q179 619 154 602T119 569T109 550Q109 549 114 549Q132 549 151 535T170 489Q170 464 154 447T109 429Z">
            </path>
            <path stroke-width="0" id="E14-MJMAIN-28"
              d="M94 250Q94 319 104 381T127 488T164 576T202 643T244 695T277 729T302 750H315H319Q333 750 333 741Q333 738 316 720T275 667T226 581T184 443T167 250T184 58T225 -81T274 -167T316 -220T333 -241Q333 -250 318 -250H315H302L274 -226Q180 -141 137 -14T94 250Z">
            </path>
            <path stroke-width="0" id="E14-MJMAIN-2E"
              d="M78 60Q78 84 95 102T138 120Q162 120 180 104T199 61Q199 36 182 18T139 0T96 17T78 60Z"></path>
            <path stroke-width="0" id="E14-MJMAIN-2212"
              d="M84 237T84 250T98 270H679Q694 262 694 250T679 230H98Q84 237 84 250Z"></path>
            <path stroke-width="0" id="E14-MJMAIN-29"
              d="M60 749L64 750Q69 750 74 750H86L114 726Q208 641 251 514T294 250Q294 182 284 119T261 12T224 -76T186 -143T145 -194T113 -227T90 -246Q87 -249 86 -250H74Q66 -250 63 -250T58 -247T55 -238Q56 -237 66 -225Q221 -64 221 250T66 725Q56 737 55 738Q55 746 60 749Z">
            </path>
          </defs>
          <g stroke="currentColor" fill="currentColor" stroke-width="0" transform="matrix(1 0 0 -1 0 0)">
            <use xlink:href="#E14-MJMATHI-61" x="0" y="0"></use>
            <g transform="translate(529,-150)">
              <use transform="scale(0.707)" xlink:href="#E14-MJMATHI-6E" x="0" y="0"></use>
              <use transform="scale(0.707)" xlink:href="#E14-MJMAIN-2B" x="600" y="0"></use>
              <use transform="scale(0.707)" xlink:href="#E14-MJMAIN-31" x="1378" y="0"></use>
            </g>
            <use xlink:href="#E14-MJMAIN-2265" x="2234" y="0"></use>
            <g transform="translate(3012,0)">
              <g transform="translate(397,0)">
                <rect stroke="none" width="473" height="60" x="0" y="220"></rect>
                <use transform="scale(0.707)" xlink:href="#E14-MJMAIN-31" x="84" y="576"></use>
                <use transform="scale(0.707)" xlink:href="#E14-MJMAIN-32" x="84" y="-536"></use>
              </g>
            </g>
            <use xlink:href="#E14-MJMAIN-28" x="4004" y="0"></use>
            <g transform="translate(4393,0)">
              <use xlink:href="#E14-MJMATHI-61" x="0" y="0"></use>
              <use transform="scale(0.707)" xlink:href="#E14-MJMAIN-31" x="748" y="-213"></use>
            </g>
            <use xlink:href="#E14-MJMAIN-2B" x="5597" y="0"></use>
            <g transform="translate(6598,0)">
              <use xlink:href="#E14-MJMATHI-61" x="0" y="0"></use>
              <use transform="scale(0.707)" xlink:href="#E14-MJMAIN-32" x="748" y="-213"></use>
            </g>
            <use xlink:href="#E14-MJMAIN-2B" x="7580" y="0"></use>
            <use xlink:href="#E14-MJMAIN-2E" x="8358" y="0"></use>
            <use xlink:href="#E14-MJMAIN-2E" x="8803" y="0"></use>
            <use xlink:href="#E14-MJMAIN-2E" x="9247" y="0"></use>
            <use xlink:href="#E14-MJMAIN-2B" x="9692" y="0"></use>
            <g transform="translate(10470,0)">
              <use xlink:href="#E14-MJMATHI-61" x="0" y="0"></use>
              <g transform="translate(529,-150)">
                <use transform="scale(0.707)" xlink:href="#E14-MJMATHI-6E" x="0" y="0"></use>
                <use transform="scale(0.707)" xlink:href="#E14-MJMAIN-2212" x="600" y="0"></use>
                <use transform="scale(0.707)" xlink:href="#E14-MJMAIN-32" x="1378" y="0"></use>
              </g>
            </g>
            <use xlink:href="#E14-MJMAIN-2B" x="12649" y="0"></use>
            <g transform="translate(13649,0)">
              <use xlink:href="#E14-MJMATHI-61" x="0" y="0"></use>
              <g transform="translate(529,-150)">
                <use transform="scale(0.707)" xlink:href="#E14-MJMATHI-6E" x="0" y="0"></use>
                <use transform="scale(0.707)" xlink:href="#E14-MJMAIN-2212" x="600" y="0"></use>
                <use transform="scale(0.707)" xlink:href="#E14-MJMAIN-31" x="1378" y="0"></use>
              </g>
            </g>
            <use xlink:href="#E14-MJMAIN-2B" x="15829" y="0"></use>
            <g transform="translate(16829,0)">
              <use xlink:href="#E14-MJMATHI-61" x="0" y="0"></use>
              <use transform="scale(0.707)" xlink:href="#E14-MJMATHI-6E" x="748" y="-213"></use>
            </g>
            <use xlink:href="#E14-MJMAIN-29" x="17882" y="0"></use>
          </g>
        </svg></span>
      <script type="math/tex">{a_{n+1}≥\frac{1}{2}(a_1+a_2+...+a_{n-2}+a_{n-1}+a_n)}</script>成立</p>
    <p><span class="MathJax_SVG" tabindex="-1" style="font-size: 100%; display: inline-block;"><svg
          xmlns:xlink="http://www.w3.org/1999/xlink" width="1.549ex" height="1.703ex" viewBox="0 -574.9 667 733.2"
          role="img" focusable="false" style="vertical-align: -0.368ex;">
          <defs>
            <path stroke-width="0" id="E16-MJAMS-2234"
              d="M273 411Q273 437 291 454T334 471Q358 471 375 454T393 411T376 368T333 351Q307 351 290 368T273 411ZM84 38Q110 38 126 21T143 -22Q143 -46 127 -64T83 -82Q57 -82 41 -65T24 -22Q24 4 41 21T84 38ZM524 -22Q524 4 541 21T584 38Q608 38 625 21T643 -22Q643 -45 627 -63T583 -82Q557 -82 541 -65T524 -22Z">
            </path>
          </defs>
          <g stroke="currentColor" fill="currentColor" stroke-width="0" transform="matrix(1 0 0 -1 0 0)">
            <use xlink:href="#E16-MJAMS-2234" x="0" y="0"></use>
          </g>
        </svg></span>
      <script type="math/tex">{\therefore}</script> 对于<span class="MathJax_SVG" tabindex="-1"
        style="font-size: 100%; display: inline-block;"><svg xmlns:xlink="http://www.w3.org/1999/xlink" width="2.685ex"
          height="2.066ex" viewBox="0 -783.2 1156 889.4" role="img" focusable="false" style="vertical-align: -0.247ex;">
          <defs>
            <path stroke-width="0" id="E17-MJMAIN-2200"
              d="M0 673Q0 684 7 689T20 694Q32 694 38 680T82 567L126 451H430L473 566Q483 593 494 622T512 668T519 685Q524 694 538 694Q556 692 556 674Q556 670 426 329T293 -15Q288 -22 278 -22T263 -15Q260 -11 131 328T0 673ZM414 410Q414 411 278 411T142 410L278 55L414 410Z">
            </path>
            <path stroke-width="0" id="E17-MJMATHI-6E"
              d="M21 287Q22 293 24 303T36 341T56 388T89 425T135 442Q171 442 195 424T225 390T231 369Q231 367 232 367L243 378Q304 442 382 442Q436 442 469 415T503 336T465 179T427 52Q427 26 444 26Q450 26 453 27Q482 32 505 65T540 145Q542 153 560 153Q580 153 580 145Q580 144 576 130Q568 101 554 73T508 17T439 -10Q392 -10 371 17T350 73Q350 92 386 193T423 345Q423 404 379 404H374Q288 404 229 303L222 291L189 157Q156 26 151 16Q138 -11 108 -11Q95 -11 87 -5T76 7T74 17Q74 30 112 180T152 343Q153 348 153 366Q153 405 129 405Q91 405 66 305Q60 285 60 284Q58 278 41 278H27Q21 284 21 287Z">
            </path>
          </defs>
          <g stroke="currentColor" fill="currentColor" stroke-width="0" transform="matrix(1 0 0 -1 0 0)">
            <use xlink:href="#E17-MJMAIN-2200" x="0" y="0"></use>
            <use xlink:href="#E17-MJMATHI-6E" x="556" y="0"></use>
          </g>
        </svg></span>
      <script type="math/tex">{\forall n}</script>均有归纳假设成立，引理得证</p>
  </blockquote>
  <p>对于分类一，显然是满足题意的。</p>
  <p>对于分类二，剩下九条线段中一定是不能再自身线段中找到都成三角形的。所以，最长的线段一定<span class="MathJax_SVG" tabindex="-1"
      style="font-size: 100%; display: inline-block;"><svg xmlns:xlink="http://www.w3.org/1999/xlink" width="5.936ex"
        height="2.671ex" viewBox="0 -835.3 2555.8 1149.8" role="img" focusable="false" style="vertical-align: -0.73ex;">
        <defs>
          <path stroke-width="0" id="E18-MJMAIN-2265"
            d="M83 616Q83 624 89 630T99 636Q107 636 253 568T543 431T687 361Q694 356 694 346T687 331Q685 329 395 192L107 56H101Q83 58 83 76Q83 77 83 79Q82 86 98 95Q117 105 248 167Q326 204 378 228L626 346L360 472Q291 505 200 548Q112 589 98 597T83 616ZM84 -118Q84 -108 99 -98H678Q694 -104 694 -118Q694 -130 679 -138H98Q84 -131 84 -118Z">
          </path>
          <path stroke-width="0" id="E18-MJMAIN-31"
            d="M213 578L200 573Q186 568 160 563T102 556H83V602H102Q149 604 189 617T245 641T273 663Q275 666 285 666Q294 666 302 660V361L303 61Q310 54 315 52T339 48T401 46H427V0H416Q395 3 257 3Q121 3 100 0H88V46H114Q136 46 152 46T177 47T193 50T201 52T207 57T213 61V578Z">
          </path>
          <path stroke-width="0" id="E18-MJMAIN-2F"
            d="M423 750Q432 750 438 744T444 730Q444 725 271 248T92 -240Q85 -250 75 -250Q68 -250 62 -245T56 -231Q56 -221 230 257T407 740Q411 750 423 750Z">
          </path>
          <path stroke-width="0" id="E18-MJMAIN-33"
            d="M127 463Q100 463 85 480T69 524Q69 579 117 622T233 665Q268 665 277 664Q351 652 390 611T430 522Q430 470 396 421T302 350L299 348Q299 347 308 345T337 336T375 315Q457 262 457 175Q457 96 395 37T238 -22Q158 -22 100 21T42 130Q42 158 60 175T105 193Q133 193 151 175T169 130Q169 119 166 110T159 94T148 82T136 74T126 70T118 67L114 66Q165 21 238 21Q293 21 321 74Q338 107 338 175V195Q338 290 274 322Q259 328 213 329L171 330L168 332Q166 335 166 348Q166 366 174 366Q202 366 232 371Q266 376 294 413T322 525V533Q322 590 287 612Q265 626 240 626Q208 626 181 615T143 592T132 580H135Q138 579 143 578T153 573T165 566T175 555T183 540T186 520Q186 498 172 481T127 463Z">
          </path>
        </defs>
        <g stroke="currentColor" fill="currentColor" stroke-width="0" transform="matrix(1 0 0 -1 0 0)">
          <use xlink:href="#E18-MJMAIN-2265" x="0" y="0"></use>
          <use xlink:href="#E18-MJMAIN-31" x="1055" y="0"></use>
          <use xlink:href="#E18-MJMAIN-2F" x="1555" y="0"></use>
          <use xlink:href="#E18-MJMAIN-33" x="2055" y="0"></use>
        </g>
      </svg></span>
    <script type="math/tex">{≥1/3}</script>。下面使用抽屉原理</p>
  <blockquote>
    <p>按照线段的长度分出两个抽屉</p>
    <p><span class="MathJax_SVG" tabindex="-1" style="font-size: 100%; display: inline-block;"><svg
          xmlns:xlink="http://www.w3.org/1999/xlink" width="5.897ex" height="3.275ex" viewBox="0 -939.5 2538.8 1410.2"
          role="img" focusable="false" style="vertical-align: -1.093ex;">
          <defs>
            <path stroke-width="0" id="E19-MJMAIN-5B" d="M118 -250V750H255V710H158V-210H255V-250H118Z"></path>
            <path stroke-width="0" id="E19-MJMAIN-31"
              d="M213 578L200 573Q186 568 160 563T102 556H83V602H102Q149 604 189 617T245 641T273 663Q275 666 285 666Q294 666 302 660V361L303 61Q310 54 315 52T339 48T401 46H427V0H416Q395 3 257 3Q121 3 100 0H88V46H114Q136 46 152 46T177 47T193 50T201 52T207 57T213 61V578Z">
            </path>
            <path stroke-width="0" id="E19-MJMAIN-33"
              d="M127 463Q100 463 85 480T69 524Q69 579 117 622T233 665Q268 665 277 664Q351 652 390 611T430 522Q430 470 396 421T302 350L299 348Q299 347 308 345T337 336T375 315Q457 262 457 175Q457 96 395 37T238 -22Q158 -22 100 21T42 130Q42 158 60 175T105 193Q133 193 151 175T169 130Q169 119 166 110T159 94T148 82T136 74T126 70T118 67L114 66Q165 21 238 21Q293 21 321 74Q338 107 338 175V195Q338 290 274 322Q259 328 213 329L171 330L168 332Q166 335 166 348Q166 366 174 366Q202 366 232 371Q266 376 294 413T322 525V533Q322 590 287 612Q265 626 240 626Q208 626 181 615T143 592T132 580H135Q138 579 143 578T153 573T165 566T175 555T183 540T186 520Q186 498 172 481T127 463Z">
            </path>
            <path stroke-width="0" id="E19-MJMAIN-2C"
              d="M78 35T78 60T94 103T137 121Q165 121 187 96T210 8Q210 -27 201 -60T180 -117T154 -158T130 -185T117 -194Q113 -194 104 -185T95 -172Q95 -168 106 -156T131 -126T157 -76T173 -3V9L172 8Q170 7 167 6T161 3T152 1T140 0Q113 0 96 17Z">
            </path>
            <path stroke-width="0" id="E19-MJMAIN-32"
              d="M109 429Q82 429 66 447T50 491Q50 562 103 614T235 666Q326 666 387 610T449 465Q449 422 429 383T381 315T301 241Q265 210 201 149L142 93L218 92Q375 92 385 97Q392 99 409 186V189H449V186Q448 183 436 95T421 3V0H50V19V31Q50 38 56 46T86 81Q115 113 136 137Q145 147 170 174T204 211T233 244T261 278T284 308T305 340T320 369T333 401T340 431T343 464Q343 527 309 573T212 619Q179 619 154 602T119 569T109 550Q109 549 114 549Q132 549 151 535T170 489Q170 464 154 447T109 429Z">
            </path>
            <path stroke-width="0" id="E19-MJMAIN-29"
              d="M60 749L64 750Q69 750 74 750H86L114 726Q208 641 251 514T294 250Q294 182 284 119T261 12T224 -76T186 -143T145 -194T113 -227T90 -246Q87 -249 86 -250H74Q66 -250 63 -250T58 -247T55 -238Q56 -237 66 -225Q221 -64 221 250T66 725Q56 737 55 738Q55 746 60 749Z">
            </path>
          </defs>
          <g stroke="currentColor" fill="currentColor" stroke-width="0" transform="matrix(1 0 0 -1 0 0)">
            <use xlink:href="#E19-MJMAIN-5B" x="0" y="0"></use>
            <g transform="translate(278,0)">
              <g transform="translate(120,0)">
                <rect stroke="none" width="473" height="60" x="0" y="220"></rect>
                <use transform="scale(0.707)" xlink:href="#E19-MJMAIN-31" x="84" y="576"></use>
                <use transform="scale(0.707)" xlink:href="#E19-MJMAIN-33" x="84" y="-535"></use>
              </g>
            </g>
            <use xlink:href="#E19-MJMAIN-2C" x="991" y="0"></use>
            <g transform="translate(1269,0)">
              <g transform="translate(286,0)">
                <rect stroke="none" width="473" height="60" x="0" y="220"></rect>
                <use transform="scale(0.707)" xlink:href="#E19-MJMAIN-32" x="84" y="576"></use>
                <use transform="scale(0.707)" xlink:href="#E19-MJMAIN-33" x="84" y="-535"></use>
              </g>
            </g>
            <use xlink:href="#E19-MJMAIN-29" x="2149" y="0"></use>
          </g>
        </svg></span>
      <script type="math/tex">{[\frac{1}{3},\frac{2}{3})}</script>,<span class="MathJax_SVG" tabindex="-1"
        style="font-size: 100%; display: inline-block;"><svg xmlns:xlink="http://www.w3.org/1999/xlink" width="5.143ex"
          height="3.275ex" viewBox="0 -939.5 2214.2 1410.2" role="img" focusable="false"
          style="vertical-align: -1.093ex;">
          <defs>
            <path stroke-width="0" id="E20-MJMAIN-5B" d="M118 -250V750H255V710H158V-210H255V-250H118Z"></path>
            <path stroke-width="0" id="E20-MJMAIN-32"
              d="M109 429Q82 429 66 447T50 491Q50 562 103 614T235 666Q326 666 387 610T449 465Q449 422 429 383T381 315T301 241Q265 210 201 149L142 93L218 92Q375 92 385 97Q392 99 409 186V189H449V186Q448 183 436 95T421 3V0H50V19V31Q50 38 56 46T86 81Q115 113 136 137Q145 147 170 174T204 211T233 244T261 278T284 308T305 340T320 369T333 401T340 431T343 464Q343 527 309 573T212 619Q179 619 154 602T119 569T109 550Q109 549 114 549Q132 549 151 535T170 489Q170 464 154 447T109 429Z">
            </path>
            <path stroke-width="0" id="E20-MJMAIN-33"
              d="M127 463Q100 463 85 480T69 524Q69 579 117 622T233 665Q268 665 277 664Q351 652 390 611T430 522Q430 470 396 421T302 350L299 348Q299 347 308 345T337 336T375 315Q457 262 457 175Q457 96 395 37T238 -22Q158 -22 100 21T42 130Q42 158 60 175T105 193Q133 193 151 175T169 130Q169 119 166 110T159 94T148 82T136 74T126 70T118 67L114 66Q165 21 238 21Q293 21 321 74Q338 107 338 175V195Q338 290 274 322Q259 328 213 329L171 330L168 332Q166 335 166 348Q166 366 174 366Q202 366 232 371Q266 376 294 413T322 525V533Q322 590 287 612Q265 626 240 626Q208 626 181 615T143 592T132 580H135Q138 579 143 578T153 573T165 566T175 555T183 540T186 520Q186 498 172 481T127 463Z">
            </path>
            <path stroke-width="0" id="E20-MJMAIN-2C"
              d="M78 35T78 60T94 103T137 121Q165 121 187 96T210 8Q210 -27 201 -60T180 -117T154 -158T130 -185T117 -194Q113 -194 104 -185T95 -172Q95 -168 106 -156T131 -126T157 -76T173 -3V9L172 8Q170 7 167 6T161 3T152 1T140 0Q113 0 96 17Z">
            </path>
            <path stroke-width="0" id="E20-MJMAIN-31"
              d="M213 578L200 573Q186 568 160 563T102 556H83V602H102Q149 604 189 617T245 641T273 663Q275 666 285 666Q294 666 302 660V361L303 61Q310 54 315 52T339 48T401 46H427V0H416Q395 3 257 3Q121 3 100 0H88V46H114Q136 46 152 46T177 47T193 50T201 52T207 57T213 61V578Z">
            </path>
            <path stroke-width="0" id="E20-MJMAIN-5D" d="M22 710V750H159V-250H22V-210H119V710H22Z"></path>
          </defs>
          <g stroke="currentColor" fill="currentColor" stroke-width="0" transform="matrix(1 0 0 -1 0 0)">
            <use xlink:href="#E20-MJMAIN-5B" x="0" y="0"></use>
            <g transform="translate(278,0)">
              <g transform="translate(120,0)">
                <rect stroke="none" width="473" height="60" x="0" y="220"></rect>
                <use transform="scale(0.707)" xlink:href="#E20-MJMAIN-32" x="84" y="576"></use>
                <use transform="scale(0.707)" xlink:href="#E20-MJMAIN-33" x="84" y="-535"></use>
              </g>
            </g>
            <use xlink:href="#E20-MJMAIN-2C" x="991" y="0"></use>
            <use xlink:href="#E20-MJMAIN-31" x="1436" y="0"></use>
            <use xlink:href="#E20-MJMAIN-5D" x="1936" y="0"></use>
          </g>
        </svg></span>
      <script type="math/tex">{[\frac{2}{3},1]}</script>
    </p>
    <p>那么显然至少有一个抽屉中有3条线段。易证明，同一个抽屉中的三条线段一定是可以构成三角形的。</p>
    <p>所以原命题得证。</p>
  </blockquote>
  <p>对于分类三，剩下10条线段，证明过程与分类二类似，不再赘述。</p>
  <hr />
  <p>按照这么推导，有没有觉得给10条结论怪怪的？</p>
  <p>是不是8条就够了呢？是不是我们哪里有问题呢？</p>
  <p>&nbsp;</p>
</body>

</html>