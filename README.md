# MapaHs
Pequeno Módulo para carregar e salvar mapas em Haskell

# Importação

é necessário ter o Cabal instalado. Se possui Haskell instalado, provavelmente já possui o Cabal, ele é instalado junto ao GHC pelo GHCUP (https://www.haskell.org/ghcup/)
Dito isso, basta baixar os arquivos desse repositório e executar ``cabal repl´´. Você estará no ghci, com MapaHS propiamente carregado. Ainda é possível carregar outros arquivos normalmente.

Caso queria importar as funções deste módulo basta escrever no topo do seu arquivo:

import Mapa

# Uso

Há duas funções disponíveis:

carregarMapa :: String -> IO Mapa
salvarMapa :: Mapa -> String -> IO Bool

e o tipo:

type Mapa = [(String, (Double, Double), [String])]

Elas devem ser usadas dessa forma:

mapa <- carregarMapa "arquivo.mapa"

resultadoSave <- salvarMapa mapa "arquivo.mapa" 

perceba o uso de "<-" ao invéz de "=".

# Exemplos

![image](https://github.com/Cubidev3/MapaHs/assets/100206395/d20afff4-7847-4b02-8870-f1668d526461)
