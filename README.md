<h1>Dasafio 1 QA Pigz</h1>

    <table border="1">
        <tr>
            <th>Funcionalidade</th>
            <th>Cenário de teste</th>
            <th>Passos</th> 
            <th>Resultado esperado</th>
        </tr>
        <tr>
            <td rowspan="4"><ol>
                <li>Cadastro de novos restaurantes</li>
            </ol></td>
            <td>Casdastro de restaurante com todos os campos preenchidos corretamente</td>
            <td>
                <ol>
                    <li>Acessar o painel de administação do sistema.</li>
                    <li>Selecionar a opção Cadastro de restaurante.</li>
                    <li>Preencher os campos obrigatórios com válidos como o nome, endereço, telefone é CNPJ.</li>
                    <li>Checar se o CNPJ informado é válido.</li>
                    <li>Verificar se o sistema exibiu a menssagem de confirmação.</li>
                    <li>É aguarda se o usuário ira ser redirecionado para lista de restaurantes cadastrados.</li>
                    <td>O restaurante foi cadastrado com sucesso.</td>
                </ol>
            </td>
        </tr>
        <tr>
            <td>Cadastro de restaurante com CNPJ inválido.</td>
            <td>
                <ol>
                    <li>Acessar o painel de administação do sistema.</li>
                    <li>Selecionar a opção Cadastro de restaurante.</li>
                    <li>Preencher os campos obrigatórios com válidos como o nome, endereço, telefone com exceção do CNPJ onde informo um valor inválido.</li>
                    <li>Digita o mesmo CNPJ inválido citado anteriormente.</li>
                    <li>Clica no botão salvar.</li>
                    <li>Verificar se a menssagem de erro é exibida, informando o CNPJ inválido.</li>
                    <li>Checar se o restaurando não e cadastrado no sistema.</li>
                </ol>
                <td>O sistema impede o cadastro de um restaurante com o CNPJ inválido.</td>
            </td>
        </tr>
        <tr>
            <td>Cadastro de restaurante com CNPJ já existente</td>
            <td>
                <ol>
                    <li>Acessar o painel de administação do sistema.</li>
                    <li>Selecionar a opção Cadastro de restaurante.</li>
                    <li>Preencher os campos obrigatórios com válidos como o nome, endereço, telefone é um CNPJ já existente no sistema.</li>
                    <li>Digita o CNPJ existente no sistema.</li>
                    <li>Clica no botão salvar.</li>
                    <li>Verifica se restorna uma menssagem de erro, informado que o CNPJ já está em uso.</li> 
                    <li>Verificar se o restaurante não foi cadastrado no sistema.</li>
                    <td>O sistema impede o cadastro de um restaurante já cadastrado no sistema.</td>
                </ol>
            </td>
        </tr>
        <tr>
            <td>Cadastro de restaurante com campos obrigatórios em branco</td>
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
