# Cadastro de novos restaurantes:

<table border="1">
    <tr>
        <th>Funcionalidade</th>
        <th>Cenário de teste</th>
        <th>Passos</th> 
        <th>Resultado esperado</th>
    </tr>
    <tr>
        <td rowspan="4">
            <ol>
                <li>Cadastro de novos restaurantes.</li>
            </ol>
        </td>
        <td>Casdastro de restaurante com todos os campos preenchidos corretamente</td>
        <td>
            <ol>
                <li>Acessar o painel de administração do sistema.</li>
                <li>Selecionar a opção Cadastro de restaurante.</li>
                <li>Preencher os campos obrigatórios com válidos como o nome, endereço, telefone e CNPJ.</li>
                <li>Checar se o CNPJ informado é válido.</li>
                <li>Verificar se o sistema exibiu a mensagem de confirmação.</li>
                <li>Aguardar se o usuário será redirecionado para a lista de restaurantes cadastrados.</li>
            </ol>
        </td>
        <td>O restaurante foi cadastrado com sucesso.</td>
    </tr>
    <tr>
        <td>Cadastro de restaurante com CNPJ inválido.</td>
        <td>
            <ol>
                <li>Acessar o painel de administração do sistema.</li>
                <li>Selecionar a opção Cadastro de restaurante.</li>
                <li>Preencher os campos obrigatórios com válidos como o nome, endereço, telefone, com exceção do CNPJ onde informo um valor inválido.</li>
                <li>Digitar o mesmo CNPJ inválido citado anteriormente.</li>
                <li>Clicar no botão salvar.</li>
                <li>Verificar se a mensagem de erro é exibida, informando o CNPJ inválido.</li>
                <li>Checar se o restaurante não é cadastrado no sistema.</li>
            </ol>
        </td>
        <td>O sistema impede o cadastro de um restaurante com o CNPJ inválido.</td>
    </tr>
    <tr>
        <td>Cadastro de restaurante com CNPJ já existente.</td>
        <td>
            <ol>
                <li>Acessar o painel de administração do sistema.</li>
                <li>Selecionar a opção Cadastro de restaurante.</li>
                <li>Preencher os campos obrigatórios com válidos como o nome, endereço, telefone e um CNPJ já existente no sistema.</li>
                <li>Digitar o CNPJ existente no sistema.</li>
                <li>Clicar no botão salvar.</li>
                <li>Verificar se retorna uma mensagem de erro, informando que o CNPJ já está em uso.</li> 
                <li>Verificar se o restaurante não foi cadastrado no sistema.</li>
            </ol>
        </td>
        <td>O sistema impede o cadastro de um restaurante já cadastrado no sistema.</td>
    </tr>
    <tr>
        <td>Cadastro de restaurante com campos obrigatórios em branco.</td>
        <td>
                <ol>
                    <li>Acessar o painel de administação do sistema.</li>
                    <li>Selecionar a opção Cadastro de restaurantes.</li>
                    <li>Deixar os campos obrigatórios em branco.</li>
                    <li>Clica no botão salvar.</li>
                    <li>Verifica se houve o retorno da menssagem de erro informado que os campos obrigatóriosdevem ser preenchidos.</li>
                    <li>Verifica se o restaurante não e cadastrado no sistema</li>
                    <td>O sistema impede o cadastro de um restaurante com campos obrigatórios em branco.</td>
                </ol>
            </td>
        </tr>
    </table>
    
# Cadastro de cardápios:

<table border="1">
    <tr>
        <th>Funcionalidade</th>
        <th>Cenário de teste</th>
        <th>Passos</th> 
        <th>Resultado esperado</th>
    </tr>
       <tr>
        <td rowspan="5">
            <ol>
                <li>Cadastro de cardápios.</li>
            </ol>
        </td>
           <td>Casdastro de cardápio com todos os campos preenchidos corretamente</td>
        <td>
            <ol>
                <li>Acessar o painel de administração do sistema.</li>
                <li>Selecionar a opção Cadastro de cardápios.</li>
                <li>Selecionar o restaurante desejado.</li>
                <li>Preencher o nome do cardápio é uma breve descrição.</li>
                <li>Preencher os campos obrigatórios de cada item do cardápio nome, descrição, preço.</li>
                <li>Clica no botão salvar.</li>
                <li>Verificar se uma menssagem de confirmação será exibida.</li>
                <li>Verificar se o usuário é redirecionado para a lista de cardápios cadastrados.</li>
            </ol>
                <td>O cardápio foi casdastrado com sucesso no sistema.</td>
    </tr>
    <tr>
        </td>
        <td>Casdastro de cardápio sem preencher o nome.</td>
        <td>
            <ol>
                <li>Acessar o painel de administração do sistema.</li>
                <li>Selecionar a opção Cadastro de cardápios.</li>
                <li>Selecionar o restaurante desejado.</li>
                <li>Deixar o campo nome em branco.</li>
                <li>Preencher os outros campos obrigatórios.</li>
                <li>Clica no botão salvar.</li>
                <li>Verificar se uma menssagem de erro será exibida informando que o nome do cardápio é obrigatório.</li>
                <li>Verificar se o cardápio não é cadastrado no sistema.</li>
            </ol>
                <td>O sistema impede o cadastro de um cardápio sem nome.</td>
        </td>
        </tr>
        <tr>
        <td>Casdastro de cardápio sem preencher o nome de um item.</td>
        <td>
            <ol>
                <li>Acessar o painel de administração do sistema.</li>
                <li>Selecionar a opção Cadastro de cardápios.</li>
                <li>Selecionar o restaurante desejado.</li>
                <li>Preencher o nome do cardápio é uma breve descrição.</li>
                <li>Preencher os campos obrigatórios de cada item do cardápio nome, exceto o nome do item.</li>
                <li>Clica no botão salvar.</li>
                <li>Verificar se ira have a menssagem de erro, informando que o nome de um item do cardápio é obrigatorio.</li>
                <li>Verificar se o cardápio não é cadastrado no sistema.</li>
            </ol>
                <td>O sistema impede o cadastro de um cardápio com item sem nome.</td>
        </td>
        </tr>
        <tr>
        <td>Casdastro de cardápio com preço inválido.</td>
        <td>
            <ol>
                <li>Acessar o painel de administração do sistema.</li>
                <li>Selecionar a opção Cadastro de cardápios.</li>
                <li>Selecionar o restaurante desejado.</li>
                <li>Preencher o nome do cardápio é uma breve descrição.</li>
                <li>Preencher os campos obrigatórios de cada item do cardápio, incluido um preço invalido.</li>
                <li>Clica no botão salvar.</li>
                <li>Verifica se uma menssagem de erro é exibida, informando que o preço de um item do cardápio é invalido.</li>
                <li>Verificar se o cardápio não é cadastrado no sistema.</li>
            </ol>
                <td>O sistema impede o cadastro de um cardápio com preço inválido.</td>
        </td>
        </tr>
        <tr>
        <td>Casdastro de cardápio com nome duplicado para o mesmo restaurante.</td>
        <td>
            <ol>
                <li>Acessar o painel de administração do sistema.</li>
                <li>Selecionar a opção Cadastro de cardápios.</li>
                <li>Selecionar o restaurante desejado.</li>
                <li>Preencher o nome do cardápio já existente do mesmo restaurante, é uma breve descrição.</li>
                <li>Preencher os campos obrigatórios de cada item do cardápio.</li>
                <li>Clica no botão salvar.</li>
                <li>Verifica se uma menssagem de erro é exibida, informando que já existe um cardápio com o mesmo nome para o restaurante selecionado.</li>
                <li>Verificar se o cardápio não é cadastrado no sistema.</li>
            </ol>
                <td>O sistema impede o cadastro de um cardápio com nome duplicado para o mesmo restaurante.</td>
        </td>
        </tr>
        
        

