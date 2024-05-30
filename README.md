# Desafio Dio -  Script para criar uma biblioteca de utilidades no Roblox Studio



**Programa:** Roblox Studio

**Código:** Lua

**Script para criar uma biblioteca de utilidades no Roblox Studio:**

lua



```lua
-- Variáveis globais
local bibliotecaDeUtilidades = {}

-- Função para adicionar uma nova utilidade à biblioteca
function bibliotecaDeUtilidades.adicionarUtilidade(nomeUtilidade, funcaoUtilidade)
    bibliotecaDeUtilidades[nomeUtilidade] = funcaoUtilidade
end

-- Função para usar uma utilidade da biblioteca
function bibliotecaDeUtilidades.usarUtilidade(nomeUtilidade, ...)
    local funcaoUtilidade = bibliotecaDeUtilidades[nomeUtilidade]
    if funcaoUtilidade ~= nil then
        return funcaoUtilidade(...)
    end
end

-- Exemplo de uso da biblioteca de utilidades
local minhaUtilidade = bibliotecaDeUtilidades.adicionarUtilidade("minhaUtilidade", function(a, b)
    return a + b
end)

local resultado = bibliotecaDeUtilidades.usarUtilidade("minhaUtilidade", 10, 20)
print(resultado) -- Imprime 30
```



#### **Observações:**

- Você pode adicionar quantas utilitárias quiser à biblioteca.
- Você pode usar as utilitárias em qualquer parte do seu jogo.
- Você pode compartilhar a biblioteca com outros desenvolvedores.

Este script criará uma biblioteca de utilitárias básicas no Roblox Studio. Você pode adicionar mais utilitárias à biblioteca conforme necessário.



**Programa:** Roblox Studio

**Código:** Lua

**Script para criar uma biblioteca de utilidades abrangente no Roblox Studio:**

lua



```lua
-- Módulo de biblioteca de utilidades
local bibliotecaDeUtilidades = {}

-- Função para adicionar uma nova utilidade à biblioteca
function bibliotecaDeUtilidades.adicionarUtilidade(nomeUtilidade, funcaoUtilidade)
    bibliotecaDeUtilidades[nomeUtilidade] = funcaoUtilidade
end

-- Função para usar uma utilidade da biblioteca
function bibliotecaDeUtilidades.usarUtilidade(nomeUtilidade, ...)
    local funcaoUtilidade = bibliotecaDeUtilidades[nomeUtilidade]
    if funcaoUtilidade ~= nil then
        return funcaoUtilidade(...)
    end
end

-- Utilitárias matemáticas
bibliotecaDeUtilidades.adicionarUtilidade("somar", function(a, b)
    return a + b
end)

bibliotecaDeUtilidades.adicionarUtilidade("subtrair", function(a, b)
    return a - b
end)

bibliotecaDeUtilidades.adicionarUtilidade("multiplicar", function(a, b)
    return a * b
end)

bibliotecaDeUtilidades.adicionarUtilidade("dividir", function(a, b)
    return a / b
end)

bibliotecaDeUtilidades.adicionarUtilidade("potencia", function(a, b)
    return a ^ b
end)

bibliotecaDeUtilidades.adicionarUtilidade("raizQuadrada", function(a)
    return math.sqrt(a)
end)

bibliotecaDeUtilidades.adicionarUtilidade("arredondar", function(a, casasDecimais)
    return math.round(a * 10^casasDecimais) / 10^casasDecimais
end)

-- Utilitárias de string
bibliotecaDeUtilidades.adicionarUtilidade("concatenar", function(...)
    local args = {...}
    return table.concat(args, "")
end)

bibliotecaDeUtilidades.adicionarUtilidade("dividirString", function(string, separador)
    return string.split(string, separador)
end)

bibliotecaDeUtilidades.adicionarUtilidade("substituirString", function(string, stringAntiga, stringNova)
    return string.gsub(string, stringAntiga, stringNova)
end)

bibliotecaDeUtilidades.adicionarUtilidade("minusculas", function(string)
    return string.lower(string)
end)

bibliotecaDeUtilidades.adicionarUtilidade("maiusculas", function(string)
    return string.upper(string)
end)

bibliotecaDeUtilidades.adicionarUtilidade("capitalizar", function(string)
    return string.gsub(string, "^%l", string.upper)
end)

-- Utilitárias de tabela
bibliotecaDeUtilidades.adicionarUtilidade("criarTabela", function(...)
    local args = {...}
    return table.create(args)
end)

bibliotecaDeUtilidades.adicionarUtilidade("adicionarTabela", function(tabela, ...)
    local args = {...}
    for i, arg in pairs(args) do
        table.insert(tabela, arg)
    end
    return tabela
end)

bibliotecaDeUtilidades.adicionarUtilidade("removerTabela", function(tabela, indice)
    table.remove(tabela, indice)
    return tabela
end)

bibliotecaDeUtilidades.adicionarUtilidade("ordenarTabela", function(tabela)
    table.sort(tabela)
    return tabela
end)

bibliotecaDeUtilidades.adicionarUtilidade("inverterTabela", function(tabela)
    table.reverse(tabela)
    return tabela
end)

-- Utilitárias de objeto
bibliotecaDeUtilidades.adicionarUtilidade("copiarObjeto", function(objeto)
    return table.copy(objeto)
end)

bibliotecaDeUtilidades.adicionarUtilidade("mesclarObjetos", function(objeto1, objeto2)
    for k, v in pairs(objeto2) do
        objeto1[k] = v
    end
    return objeto1
end)

bibliotecaDeUtilidades.adicionarUtilidade("obterChavesObjeto", function(objeto)
    return table.keys(objeto)
end)

bibliotecaDeUtilidades.adicionarUtilidade("obterValoresObjeto", function(objeto)
    return table.values(objeto)
end)

-- Exemplo de uso da biblioteca de utilidades
local resultado = bibliotecaDeUtilidades.usarUtilidade("somar", 10, 20)
print(resultado) -- Imprime 30

local resultado = bibliotecaDeUtilidades.usarUtilidade("concatenar", "Olá", " ", "mundo!")
print(resultado) -- Imprime "Olá mundo!"

local resultado = bibliotecaDeUtilidades.usarUtilidade("ordenarTabela", {5, 2, 1, 4, 3})
print(resultado) -- Imprime {1, 2, 3, 4, 5}
```



#### **Observações:**

- Este script cria uma biblioteca de utilidades abrangente que inclui utilitárias matemáticas, de string, de tabela e de objeto.
- Você pode adicionar mais utilitárias à biblioteca conforme necessário.
- Você pode usar as utilitárias em qualquer parte do seu jogo.
- Você pode compartilhar a biblioteca com outros desenvolvedores.

Este script criará uma biblioteca de utilidades abrangente no Roblox Studio que pode ser usada para melhorar a eficiência e a qualidade do seu código.





## **Metodo de construção**



#### **Como criar jogos Roblox:**

1. **Abra o Roblox Studio.**
2. **Clique no botão \**Criar novo\**.**
3. **Selecione um modelo para o seu jogo.**
4. **Clique no botão \**Criar\**.**
5. **Comece a criar seu jogo!**



Você pode usar as ferramentas no Roblox Studio para criar seu mundo, adicionar objetos e personagens e escrever scripts para controlar o comportamento do jogo.



#### **Aqui estão algumas dicas para criar jogos Roblox:**

- **Comece pequeno.** Não tente criar um jogo muito complexo em seu primeiro projeto.
- **Use os recursos disponíveis.** O Roblox Studio possui uma ampla variedade de ferramentas e recursos para ajudá-lo a criar seu jogo.
- **Aprenda com os outros.** Existem muitos recursos online e comunidades onde você pode aprender sobre o desenvolvimento de jogos Roblox.
- **Seja criativo!** O Roblox oferece infinitas possibilidades para criar jogos únicos e divertidos.



#### **Aqui estão alguns jogos Roblox populares que você pode criar:**

- **Jogos de aventura:** Explore mundos diferentes, resolva quebra-cabeças e lute contra inimigos.
- **Jogos de construção:** Crie seus próprios mundos e estruturas.
- **Jogos de corrida:** Corra contra outros jogadores ou contra o relógio.
- **Jogos de tiro:** Atire em inimigos e complete missões.
- **Jogos de RPG:** Crie seu próprio personagem e embarque em uma jornada épica.



#### **Depois de criar seu jogo, você pode publicá-lo no Roblox para que outras pessoas possam jogá-lo.**



#### **Observações:**

- O Roblox Studio é gratuito para usar.
- Você pode encontrar muitos tutoriais e recursos online para ajudá-lo a aprender como criar jogos Roblox.
- Seja paciente e persistente. Criar jogos Roblox pode ser desafiador, mas também é muito recompensador.





### **Programas:**

- Roblox Studio
- Blender
- GIMP
- Audacity



#### **Códigos:**

- Lua (linguagem de script do Roblox)
- Python
- C++
- HTML
- CSS



#### **Apps:**

- Roblox Mobile
- Roblox Player
- Roblox Creator Companion
- Roblox Studio Mobile



#### **Como usar esses programas, códigos e apps para criar uma experiência no Roblox:**



- **Roblox Studio:** Use o Roblox Studio para criar e editar experiências do Roblox.
- **Blender:** Use o Blender para criar modelos e animações 3D para suas experiências do Roblox.
- **GIMP:** Use o GIMP para criar e editar imagens para suas experiências do Roblox.
- **Audacity:** Use o Audacity para criar e editar áudio para suas experiências do Roblox.
- **Lua:** Use a linguagem de script Lua para programar suas experiências do Roblox.
- **Python:** Use Python para criar scripts e plugins para suas experiências do Roblox.
- **C++:** Use C++ para criar plugins de alto desempenho para suas experiências do Roblox.
- **HTML:** Use HTML para criar interfaces de usuário personalizadas para suas experiências do Roblox.
- **CSS:** Use CSS para estilizar as interfaces de usuário personalizadas de suas experiências do Roblox.
- **Roblox Mobile:** Use o Roblox Mobile para jogar experiências do Roblox em seu dispositivo móvel.
- **Roblox Player:** Use o Roblox Player para jogar experiências do Roblox em seu computador.
- **Roblox Creator Companion:** Use o Roblox Creator Companion para criar e gerenciar suas experiências do Roblox em seu dispositivo móvel.
- **Roblox Studio Mobile:** Use o Roblox Studio Mobile para criar e editar experiências do Roblox em seu dispositivo móvel.



#### **Observações:**

- Você não precisa usar todos esses programas, códigos e apps para criar uma experiência no Roblox.
- Você pode usar os programas, códigos e apps que melhor se adequam às suas necessidades e habilidades.
- Há muitos recursos disponíveis online para ajudá-lo a aprender como usar esses programas, códigos e apps.





### **Vide site:**

Hands-on: Criando um Jogo de Sobrevivência no Roblox   



#### Criando uma Biblioteca de Utilidades

 https://github.com/sscastilho/desafio-roblox-

https://www.roblox.com/games/11540492058/Survival-Game-SSC

https://tecnobits.com/pt/como-colocar-roblox-em-tela-cheia-no-pc/

https://clubedovideogame.com.br/melhores-jogos-do-roblox/

https://create.roblox.com/
