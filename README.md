# Dasafio 1 QA Pigz

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
                <li>Cadastro de novos restaurantes</li>
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
        <td>Cadastro de restaurante com CNPJ já existente</td>
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
        <td>Cadastro de restaurante com campos obrigatórios em branco</td
