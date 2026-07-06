<<<<<<< HEAD
# Credit Card Fraud Detection

**Проект по обнаружению мошеннических транзакций с помощью машинного обучения**

## Цель проекта
Разработать модель, способную с высокой точностью выявлять мошеннические операции по кредитным картам при крайне сильном дисбалансе классов (всего **0.17%** фрода).

## Основные результаты
- **Лучшая модель**: XGBoost
- **F1-score (fraud)**: **0.85**
- **Recall (fraud)**: 0.84
- **Precision (fraud)**: 0.86
- **PR-AUC**: 0.85
- Пропущено всего **16** мошеннических транзакций из 98 на тестовой выборке

## Ключевые особенности проекта
- Глубокий EDA с бизнес-выводам
- Обработка сильного дисбаланса классов (`scale_pos_weight`, стратифицированный split)
- Feature Engineering (`Hour`, `Amount_log`, взаимодействия ключевых V-признаков)
- Анализ важности признаков
- Визуализация обучения (Loss Curve и Learning Curve)

## Структура проекта
Credit-Card-Fraud-Detection/
├── data/
│   └── creditcard.csv                 # исходные данные
├── notebooks/
│   └── Credit_Card_Fraud_Detection.ipynb   # основной ноутбук
├── models/                            # (опционально)
│   ├── xgboost_fraud_model.pkl
│   └── scaler.pkl
├── requirements.txt
└── README.md

## Как запустить
```bash
# 1. Клонировать репозиторий
git clone <ваш_репозиторий>
cd Credit-Card-Fraud-Detection

# 2. Установить зависимости
pip install -r requirements.txt

# 3. Запустить Jupyter
jupyter notebook
Откройте файл notebooks/Credit_Card_Fraud_Detection.ipynb

Технологии:
Python 3
pandas, numpy
scikit-learn, XGBoost
matplotlib, seaborn
imbalanced-learn

Выводы:
Наиболее важные признаки: V14, V12, V17, V10
Мошеннические транзакции чаще происходят в ночное время
Лог-преобразование суммы и создание взаимодействий признаков заметно улучшили качество модели

Дальнейшая работа:
Интерпретация модели с помощью SHAP
Подбор оптимального порога под бизнес-метрики
Ensemble моделей
Деплой модели (FastAPI / Flask)
=======
# credit-card-fraud-detection
Fraudulent transaction detection model (XGBoost, F1-score 0.85)
>>>>>>> d8feeef3fb221aa2fd37de4701201aaadb1e5ed8
