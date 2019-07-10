#Instruções
------

##1. Requisições

**1.1. Criar Rota: Arquivo - *Web.php* para Controller**
>Route::get('nome', 'User\UserController@listRole');

**1.2. Abrindo o arquivo controller (UserController.php)**
- Colocar o use 'App\Intgrations\Porteira\Services\NomeDoArquivo'
- Criar função nova (copiar uma que já existe)
>public function listRole (...)

**1.3. Criar arquivo PHP dentro da pagina '..\Porteira'**
- Copiar arquivo de Ex: ListRole.php / ListProfile.php
- Alterar caminho da rota
``` 
public function defineRoute(){
    return 'endereco' *endereco precisa ser disponibilizado*
}
```
- Alterar no mesmo arquivo o nome da class
>class ListRole extends ...

**1.4 No arquivo do componente Ex: ComboboxPerfis.vue**
- Alterar url ="nomeDaRotaCriada"
- Alterar label="nome da data que quer que apareça retornando do json"

------



##2. Subir arquivos para homologação (passo-a-passo)

git | Função
------------ | -------------
git pull --all | *Puxa todos os arquivos para atualizar*
git branch -a  | *lista todas as branchs*
git checkout homologacao | *troca para a branch homologação*
git merge dev | *Pega tudo da branch dev e passa para homologação*
git push origin homologacao | *Envia tudo de homologação*

------

##3.













