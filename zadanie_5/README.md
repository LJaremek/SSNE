Zadanie będzie polegało na stworzeniu modelu generatywnego który generował będzie nowe obrazki przedstawiające znaki drogowe. Do wyboru mają Państwo dowolny model generatywny (VAE, GAN inne opcje o których nie wspominaliśmy jak GLOW czy VAEGAN). Zbiór danych udestępniony jest przez office 365 (trafic_32.zip) i ma taką samą strukturę jak poprzednio (zgodną z domyślnymi ustawieniami ImageFolderu). Znaki podzielone są na klasy, które jak najbardziej mogą Państwo wykorzystywać do generowania próbek. Tym razem zamiast predykcji proszę o zwrócenie mi kodu z implementacją eksperymentów i przykładowe 1000 wygenerowanych za pomocą Państwa metody próbek.
Wygenerowane obrazki, proszę zapisywać po prostu w formie torchowego tensora (na cpu, po detach, czyli np. wykonując komendę torch.save(generated_imgs.cpu().detach(), "poniedzialek_nazwisko1_nazwisko2.pt")).
Tensor zgodnie z konwencją powinien mieć wymiary [1000,3,32,32]

Ewaluacja:
- Wygenerowane obrazki porównywał będę do zbioru testowego za pomocą metryki Frechet Inception Distance. Jeżeli chcieliby Państwo z niej skorzystać do ewaluacji swoich modeli, to odsyłam do repozytorium z wygodną implementacją: https://github.com/mseitzer/pytorch-fid
- W zbiorze testowym obrazki mają ten sam rozkład klas co w treningowym
- Proszę pamiętać o denormalizacji próbek :)

1000 obrazków w torchowym tensorze zajmuje około 15MB, myślę że teamsy powinny sobie z tym poradzić, w razie problemów proszę o kontakt.
