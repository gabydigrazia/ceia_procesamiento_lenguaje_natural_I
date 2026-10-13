# Procesamiento de Lenguaje Natural I

**Estudiante:** a2517 - Gabriela Di Grazia  
**Docente:** Josselyn Ordóñez  
**Carrera:** CEIA - FIUBA

## Desafíos

| Desafío | Tema | Notebook |
|---|---|---|
| 1 | Vectores de documentos (TF-IDF / Naive Bayes) | [Desafio_1_Gabriela_Di_Grazia.ipynb](Desafio_1_Gabriela_Di_Grazia.ipynb) |
| 2 | Custom embeddings con Gensim | [Desafio_2_Gabriela_Di_Grazia.ipynb](Desafio_2_Gabriela_Di_Grazia.ipynb) |
| 3 | Modelo de lenguaje por caracteres (LSTM) | [Desafio_3_Gabriela_Di_Grazia.ipynb](Desafio_3_Gabriela_Di_Grazia.ipynb) |
| 4 | Traductor seq2seq EN→ES (LSTM) | [Desafio_4_Gabriela_Di_Grazia.ipynb](Desafio_4_Gabriela_Di_Grazia.ipynb) |

## Desafío 2

Embeddings de palabras con **Word2Vec (Skip-gram, Gensim)** sobre un corpus propio: *Pride and Prejudice* (Jane Austen) desde [Project Gutenberg](https://www.gutenberg.org/ebooks/1342).

La notebook incluye el ejemplo de clase (canciones) y la resolución: limpieza del libro, entrenamiento, términos más y menos similares, reducción a 2D con t-SNE (`MAX_WORDS = 80`) e inspección de grupos (personajes, familia, matrimonio).

## Desafío 3

Modelo de lenguaje **por caracteres** (Keras / TensorFlow) sobre el mismo corpus del Desafío 2 (*Pride and Prejudice*). LSTM many-to-many con `Embedding`, perplejidad en validación (`PplCallback`), generación greedy / beam search / muestreo con temperatura, e interfaz Gradio.

Notebook ejecutada: [Desafio_3_Gabriela_Di_Grazia.ipynb](Desafio_3_Gabriela_Di_Grazia.ipynb).

## Desafío 4

Traductor **inglés → español** (seq2seq LSTM, Keras), replicando el `Traductor.ipynb` de la clase 6 y extendiéndolo: 30 000 pares `spa-eng` (vs 10 000), secuencias más largas, comparación de 128 vs 256 unidades LSTM, GloVe en el encoder, greedy y beam search.

Notebook: [Desafio_4_Gabriela_Di_Grazia.ipynb](Desafio_4_Gabriela_Di_Grazia.ipynb). Ejecutar en **Colab con GPU**.
