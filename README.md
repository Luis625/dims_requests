# dims_requests
clone this repository and enter it
git clone https://github.com/uiot/UV-Covid.git
cd UV-Covid

## create and start a virtualenv

virtualenv venv
source venv/bin/activate # Linux
./venv/Scripts/activate # Windows
pip install the requirements
pip install -r requirements.txt



## deactivate
deactivate


## TODO

add more devices according to chipset
create link between chipset and device (chipset x = id y)
split values into columns
prep data: convert cm to %, send only needed fields 
configure final csv
export to google sheets



# data goal
[id,filling percentual,date,battery level]
id -> linkink id with the chipset (future can be a key sent to dims)
from millis (https://currentmillis.com/) to ISO
data received + "%"
data received converted to % 



# infra, notes 
alguns dos devices manda um post pro heroku e as vezes manda a aplicação serveless rodar

conductor: evolução do cron, além de setar o tempo
conductor workflow definition
ele espera alguem dar um get no condutctor local host com o id da arvore criada
entende como start e roda todo o diagrama
no front define o q é um sucesso, um erro

serveless é um transistor, ele so liga quando alguem manda
no serveless coloca uma inteligencia
qual foi a ultima hora q rodou 

linux tem o cron

criar um codigo que consulta o dado do dims e joga num google sheets
dps começa a pensar em expor uma porta pra engatilhar

concentrador no meio, fica olhando o heroku, usa o conector externo 

vantagem do google sheets: manutenção, nome do google, plataforma gerenciada

hardware sua responsabilidade, software tb como laboratorio
tudo paas ou saas
n tem responsabilidade como responsabilidade