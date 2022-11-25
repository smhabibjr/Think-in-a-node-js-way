## Table of Contents

- [Project Description](#project-description)
- [Technologies and Programing Languages](#technologies-and-programming-languages)
- Frontend Design
  - [Frontend Design HTML](#frontend-design-html)
  - [Frontend Design CSS](#frontend-design-css)
  - [Frontend Design JavaScript](#frontend-design-javascript)
- Backend
  - [Backend Handling with PHP](#backend-handling-with-php)
- [Contact](#contact)

<!-- HOW TO RUN -->
## Project Description

## Technologies and Programming Languages



## Frontend Design HTML

```html
<div id="overDiv">
        <div id="formPanel">
            <ul class="dynamicButtonList">
                <?php while ($res = mysql_fetch_row($result)) { ?>
                    <li class='list_item'>
                        <span class="input-text-1-wtp pdfPreview button-gray-1-wtp button-1-wtp"
                              data-url="<?php echo "/eins/html/" . $res[2]; ?>">
                            <span class="input-text-1-wtp pdfPreviewText">
                                <?php echo utf8_decode($res[1]); ?>
                            </span>
                        </span>
                        <div id="delete_<?php echo $res[0]; ?>" class="deletePdf button-1-wtp">
                            <span class='ui-icon ui-icon-trash deleteIcon '></span>
                        </div>
                    </li>
                <?php } ?>
            </ul>
        </div>
        <div id="buttonPanel">
            <div class="button-1-wtp" id="newChecklist">
                Checkliste hinzufügen
            </div>
            <div id="displayDocuWrap">
                <div id="displayDocu" class="button-gray-1-wtp button-1-wtp">
                    Dokumentation anzeigen
                </div>
            </div>
        </div>
    </div>
```
<sup align="right"><a href="#table-of-contents">Go to top</a></sup>

## Frontend Design CSS

[![portfolio](https://img.shields.io/badge/my_portfolio-000?style=for-the-badge&logo=ko-fi&logoColor=white)](https://katherineoelsner.com/)
[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/)
[![twitter](https://img.shields.io/badge/twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white)](https://twitter.com/)

