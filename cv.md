# Dmitry Sysoyev
## Contacts
* Location: Moscow, Russia
* Phone: [+7-925-618-58-94](tel:79256185894)
* Email: [mr.thir13enth@gmail.com](mailto:mr.thir13enth@gmail.com)
* Telegram: [@dmitry_thirteenth](https://t.me/Dmitry_Thirteenth)
* GitHub: [@mrthirteenth](https://github.com/mrThirteenth)
## About Me
I am a hard working, honest individual. I am a good timekeeper, always willing to learn new skills. I am friendly, helpful and polite, have a good sense of humour. I am able to work independently in busy environments and also within a team setting. I am outgoing and tactful, and able to listen effectively when solving problems.
## Education: 
* University: Moscow State University of Instrument Engineering and Computer Science
Courses:
* [CS50 lectures](https://www.youtube.com/channel/UCcabW7890RKJzL968QWEykA)
* [FreeCodeCamp](https://www.freecodecamp.org/) - Responsive Web Design
## Skills
* HTML5, CSS3/SASS/SCSS/BEM, GULP4
* JavaScript Basics
* PHP, XSLT (template engine)
* PHPStorm, WebStorm, VS Code
* Git, GitHub, Bitbacket, Jira, Trello, Confluence
* Adobe Photoshop, Figma
* Bash, server administration
## Code Example
JS:
```
$(document).ready(function() {
    $('#js_send_pdf_form').submit(function(){
        let message = 'Получить презентацию объекта';
        let name = $('[name = name]').val();
        let email = $('[name = email]').val();
        let form = $(this);
        $.ajax({
            url: "/tools/create_pdf/index.php",
            type: "GET",
            cache: false,
            data: form.serialize(),
            dataType: "html",
            contentType: "application/x-www-form-urlencoded;charset=ISO-8859-15",
            success: function (response) {    
                console.log('response = '+response);
                console.log(name);
                console.log(email);
                  if (response == '1') { 
                    Comagic.addOfflineRequest({
                        name: name,
                        email: email,
                        message: message
                    });
                    form.html('<p class="popup__desc">Мы отправили pdf файл на ваш E-mail</p>');
                  } else {
                      $('#js_send_pdf_file_error').show();
                  }
            }
        });
        return false;
    });
});
```
PHP:
```
public function makeWordForms($count, $text_forms) 
{
    $n = abs($count) % 100;
    $n1 = $count % 10;
    if ($n > 10 && $n < 20) { return $text_forms[2]; }
    if ($n1 > 1 && $n1 < 5) { return $text_forms[1]; }
    if ($n1 == 1) { return $text_forms[0]; }
    return $text_forms[2];
}
```
## Experience
Project examples as part of the Upmix team:
[grand-mozaika.ru](https://grand-mozaika.ru), [antarescompany.ru](https://antarescompany.ru), [letoestate.ru](https://letoestate.ru), [one-estate.ru](https://one-estate.ru), [koka.press](https://koka.press), [avva-rus.ru](https://avva-rus.ru), [ecofuril.ru](https://ecofuril.ru), [ecofucin.ru](https://ecofucin.ru)
## English
* Russian - **native speaker**
* English - **A2**