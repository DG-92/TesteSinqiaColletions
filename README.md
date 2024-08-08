# Cenários de testes

# Testes de Caminho Feliz 
Esses testes focam nos cenários em que tudo ocorre conforme o esperado, sem erros ou falhas.

# Criação de Recursos (POST)

# Verificar se a criação de um novo recurso funciona corretamente com todos os campos válidos.
Confirmar se a resposta contém o status 201 (Created) e o corpo esperado.
Recuperação de Recursos (GET)

# Recuperar um recurso existente usando um ID válido.
Verificar se o status da resposta é 200 (OK) e se os dados retornados estão corretos.
Atualização Total de Recursos (PUT)

# Atualizar completamente um recurso existente com dados válidos.
Confirmar que o status da resposta é 200 (OK) e que os dados foram atualizados corretamente.
Atualização Parcial de Recursos (PATCH)

# Executar uma atualização parcial em um recurso com campos válidos.
Verificar se o status da resposta é 200 (OK) e que apenas os campos fornecidos foram atualizados.
Exclusão de Recursos (DELETE)

# Excluir um recurso existente usando um ID válido.
Verificar se o status da resposta é 204 (No Content) e se o recurso foi realmente removido.
Testes de Caminhos Alternativos (Alternate Paths)
Esses testes lidam com cenários em que algo inesperado ou incorreto ocorre.

# Criação de Recursos (POST)

# Tentar criar um recurso com dados faltantes ou inválidos (ex. campos obrigatórios ausentes).
Verificar se o status da resposta é 400 (Bad Request) e se a mensagem de erro é apropriada.
Recuperação de Recursos (GET)

# Tentar recuperar um recurso inexistente ou com um ID inválido.
Verificar se o status da resposta é 404 (Not Found).
Atualização Total/Parcial (PUT/PATCH)

# Tentar atualizar um recurso inexistente.
Verificar se a resposta retorna 404 (Not Found).
Tentar atualizar com dados inválidos ou incompletos, e verificar se o status da resposta é 400 (Bad Request).
Exclusão de Recursos (DELETE)

# Tentar excluir um recurso inexistente.
Confirmar se a resposta é 404 (Not Found).
Autenticação e Autorização

# Acessar a API sem fornecer credenciais ou com credenciais inválidas.
Verificar se a resposta retorna 401 (Unauthorized) ou 403 (Forbidden) conforme aplicável.
Validação de Limites e Restrições

# Testar os limites, como tamanhos máximos de campos e número máximo de registros que podem ser criados.
Verificar se a resposta retorna 413 (Payload Too Large) ou 429 (Too Many Requests) quando aplicável.
