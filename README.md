# ArtMl-Autoencoder-Som
Banco de Dados Real de Imagens com Autoencoder e Mapa Autoajustável (SOM) para Agrupamento de Fotos de uma Galeria de Arte de Nova York

Introdução: 

Este projeto acadêmico é o trabalho final da disciplina de mestrado da UFBA (Universidade Federal da Bahia) na disciplina de Tópicos em Inteligência Computacional III. Neste projeto, trabalhamos com um banco de dados real de imagens, utilizando técnicas de processamento de imagens e aprendizado de máquina para agrupar fotos de uma galeria de arte de Nova York.

Banco de Dados: 

O banco de dados utilizado neste projeto foi retirado da National Gallery Of Art de Nova York. Os dados estão disponíveis publicamente no link https://raw.githubusercontent.com/NationalGalleryOfArt/opendata/main/data/published_images.csv. Esse banco de dados contém uma grande quantidade de imagens, totalizando cerca de 104 gigabytes de dados. No entanto, para facilitar o processamento e a análise, realizamos um tratamento dos dados e reduzimos o banco para aproximadamente 1,4 gigabytes, mantendo apenas as imagens na dimensão de 32x32.


Técnicas Utilizadas:

1. Tratamento de Dados: Antes de prosseguir com as etapas de análise, realizamos um tratamento dos dados para garantir a qualidade e a usabilidade das imagens. Isso incluiu a remoção de imagens corrompidas ou inválidas, a padronização do formato e tamanho das imagens, bem como a redução do tamanho do banco de dados para facilitar a manipulação.
    
    
2. Autoencoder: Utilizamos a técnica de autoencoder para extrair características relevantes das imagens do banco de dados. O autoencoder é uma rede neural que aprende a codificar uma imagem em um espaço latente de dimensionalidade inferior e, em seguida, decodifica a imagem a partir desse espaço latente. Isso permite que o autoencoder aprenda uma representação compacta das imagens, capturando as informações mais importantes para a reconstrução.
    
    
3. Mapa Autoajustável (SOM): Além do autoencoder, implementamos um Mapa Autoajustável, também conhecido como Self-Organizing Map (SOM). A SOM é uma técnica de aprendizado não supervisionado que mapeia os dados em um espaço bidimensional ou tridimensional, preservando as relações topológicas entre os dados originais. Neste projeto, utilizamos a SOM para agrupar as imagens em diferentes regiões do mapa, com base em suas características semelhantes aprendidas pelo autoencoder.
    
    
Resultados e Conclusões: 

Após a aplicação do autoencoder e da SOM, obtivemos resultados interessantes. As imagens foram agrupadas em diferentes regiões do mapa, refletindo suas semelhanças e características compartilhadas. Isso possibilita a exploração eficiente do banco de dados, facilitando a busca por imagens semelhantes e a descoberta de padrões interessantes.


Por fim, gostaríamos de ressaltar que a implementação do autoencoder e da SOM foi realizada sem o uso da biblioteca "minisom", visando uma maior compreensão e controle sobre o processo.


Projeto realizado em parceria com João Pedro Neto.
