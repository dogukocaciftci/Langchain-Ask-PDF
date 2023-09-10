# Langchain Ask PDF 

Benden istenen aslında bir PDF dosyasını okuyup, kullanıcının sorduğu soruya cevap veren bir API oluşturmaktı fakat ben bunu Postman'de çalıştırmaktan ziyade bir web uygulaması olarak yapmak istedim. Bu yüzden de Streamlit kullandım.

Öncelikle proje için gereken kütüphaneleri indiriyoruz.
```
pip install -r requirements.txt
```
## Nasıl Çalışır?

Uygulama PDF'yi okur ve metni daha sonra LLM'ye beslenebilecek daha küçük parçalara böler. Parçaların vektör temsillerini oluşturmak için OpenAI yerleştirmelerini kullanır. Uygulama daha sonra kullanıcının sorduğu soruya semantik olarak benzeyen parçaları bulur ve bir yanıt oluşturmak için bu parçaları LLM'ye iletir.

Uygulama, GUI'yi oluşturmak için Streamlit'i ve LLM için Langchain'i kullanıyor.


## Kullanım

Uygulamayı kullanmak için, Streamlit CLI ile 'main.py' dosyasını çalıştırın (streamlit'i yükledikten sonra):

```
streamlit run app.py
```
Eğer kendi API Key'inizi kullanmak istiyorsanız, Langchain API Key'inizi '.env' dosyasında değiştirmeniz gerekmektedir.


