Практичне заняття 9. PyTorch MNIST

Мета роботи:
Дослідити, як розмір навчального набору MNIST впливає на точність та час навчання моделей Net_Linear і Net_Conv.

Результати експериментів:
Net_Linear, divider=1, dataset_size=60000, accuracy=0.9575, time=21.45 sec
Net_Conv, divider=1, dataset_size=60000, accuracy=0.9826, time=171.26 sec
Net_Linear, divider=2, dataset_size=30000, accuracy=0.9453, time=9.54 sec
Net_Conv, divider=2, dataset_size=30000, accuracy=0.9808, time=83.23 sec
Net_Linear, divider=4, dataset_size=15000, accuracy=0.918, time=4.9 sec
Net_Conv, divider=4, dataset_size=15000, accuracy=0.9734, time=38.27 sec
Net_Linear, divider=8, dataset_size=7500, accuracy=0.9083, time=2.28 sec
Net_Conv, divider=8, dataset_size=7500, accuracy=0.9441, time=19.01 sec

Висновок:
При зменшенні розміру навчального набору точність моделей зазвичай зменшується.
Модель Net_Conv зазвичай показує кращу точність, бо вона краще працює із зображеннями.
Модель Net_Linear навчається швидше, але може давати нижчу точність.
Чим більший навчальний набір, тим більше часу потрібно для навчання.
Основний компроміс полягає в тому, що більший датасет дає кращу точність, але потребує більше часу.
Для покращення точності на малих наборах можна збільшити кількість епох, використати аугментацію даних або покращити архітектуру моделі.
