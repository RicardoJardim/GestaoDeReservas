# Website de Gestão de reservas e pacientes em clínica privada 

Este projeto consiste num website para gestão de reversas num ambiente de uma clinica, com o objectivo de criar uma ligação mais eficiente e intuitiva entre  as  clinicas  e  os  utentes,  focando-se,  essencialmente,  nas  melhorias do sistema de reservas. 

![alt text](https://github.com/RicardoJardim/GestaoDeReservas/blob/main/diagramacontextual.png "Diagrama")

## Tecnologias
- Laravel
- JQuery
- SASS
- AJAX
- Google Calendar

## Comandos base de dados
//Commandos da Base de dados

base de dados -> Clinic_db

php artisan migrate --seed //Faz migrations de todas as tabelas da base de dados e preenche com dados que estão guardados na seed

php artisan migrate:reset //Se quiserem resetar a base de dados

Já fiz alguns teste e até agora parece que as ligações estão bem feitas

Composer install
# Styling SCSS

<!-- STYLING SCSS -->

Sempre que for preciso mudar o CSS utilizar a pasta do "resources" para mudar o scss -> "npm run watch-poll" para copilar scss para css
Caso nao funcione na primeira vez, é necessário realizar "npm install" e de seguida "npm run dev". Por fim realizar o passo em cima.

Adiconar no blade.php <!-- <link href="{{ mix('/css/app.css') }}" rel="stylesheet"> --> para funcionar
Os ficheiro _nome.scss sao ficheiros que podem ser importados para um ficheiro principal
É possivel criar um ficheiro principal diferente do app.scss, basta criar um sem o _

Para adicionar um novo ficheiro temos que ir ao ficheiro webpack.mix.js e adicionar .sass('resources/sass/nome.sass', 'public/css/nome'); logo depois correr o codigo "npm run dev"

Para tornar mais pratico criar 2 terminais

Ta feito de maneira a que App -> css do Guest ; Client -> css do cliente ; Employee -> css do Funcionario

\_Variables -> Uso global

# Estrutura

Gest -> utiliza layout app.blade.php
Funcionario -> utiliza layout employee.blade.php
Client -> utiliza layout client.blade.php

# Paginate

Verificar a paginação para as paginas do funcionário
