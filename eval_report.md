# Evaluation Report

## Model Performance

BART Model Metrics:
-------------------
                       precision    recall  f1-score   support

100_NIGHT_TRIAL_OFFER       1.00      0.44      0.62        18
   ABOUT_SOF_MATTRESS       0.40      0.73      0.52        11
         CANCEL_ORDER       1.00      0.80      0.89        10
        CHECK_PINCODE       1.00      0.10      0.18        10
                  COD       0.41      0.92      0.56        12
           COMPARISON       0.38      0.73      0.50        11
    DELAY_IN_DELIVERY       0.82      0.82      0.82        11
         DISTRIBUTORS       0.80      0.12      0.21        34
                  EMI       0.62      0.72      0.67        25
        ERGO_FEATURES       0.21      0.45      0.29        11
             LEAD_GEN       0.00      0.00      0.00        21
        MATTRESS_COST       0.69      0.41      0.51        22
               OFFERS       0.19      1.00      0.31        10
         ORDER_STATUS       0.77      0.48      0.59        21
       ORTHO_FEATURES       0.50      0.24      0.32        17
              PILLOWS       0.42      1.00      0.59        10
     PRODUCT_VARIANTS       0.75      0.14      0.24        21
      RETURN_EXCHANGE       0.13      0.21      0.16        14
   SIZE_CUSTOMIZATION       0.88      0.78      0.82         9
             WARRANTY       0.48      1.00      0.65        10
   WHAT_SIZE_TO_ORDER       0.67      0.20      0.31        20

             accuracy                           0.46       328
            macro avg       0.58      0.54      0.46       328
         weighted avg       0.59      0.46      0.43       328

Accuracy: 0.4573170731707317

FLAN-T5 Model Metrics:
----------------------
                       precision    recall  f1-score   support

100_NIGHT_TRIAL_OFFER       1.00      0.83      0.91        18
   ABOUT_SOF_MATTRESS       0.77      0.91      0.83        11
         CANCEL_ORDER       0.71      1.00      0.83        10
        CHECK_PINCODE       1.00      0.80      0.89        10
                  COD       0.85      0.92      0.88        12
           COMPARISON       1.00      0.36      0.53        11
    DELAY_IN_DELIVERY       0.77      0.91      0.83        11
         DISTRIBUTORS       0.62      0.15      0.24        34
                  EMI       0.85      0.68      0.76        25
        ERGO_FEATURES       0.64      0.82      0.72        11
             LEAD_GEN       0.00      0.00      0.00        21
        MATTRESS_COST       0.52      0.55      0.53        22
               OFFERS       0.12      1.00      0.22        10
         ORDER_STATUS       0.95      0.90      0.93        21
       ORTHO_FEATURES       1.00      0.41      0.58        17
              PILLOWS       0.83      1.00      0.91        10
     PRODUCT_VARIANTS       0.80      0.19      0.31        21
      RETURN_EXCHANGE       0.93      0.93      0.93        14
   SIZE_CUSTOMIZATION       0.28      1.00      0.44         9
             WARRANTY       1.00      1.00      1.00        10
   WHAT_SIZE_TO_ORDER       0.00      0.00      0.00        20

             accuracy                           0.59       328
            macro avg       0.70      0.68      0.63       328
         weighted avg       0.68      0.59      0.58       328

Accuracy: 0.5884146341463414



DeBERTa Small Long NLI Model Metrics:
------------------------

Classification Report:
                       precision    recall  f1-score   support

100_NIGHT_TRIAL_OFFER       0.67      0.11      0.19        18
   ABOUT_SOF_MATTRESS       0.22      0.64      0.33        11
         CANCEL_ORDER       1.00      0.90      0.95        10
        CHECK_PINCODE       1.00      0.70      0.82        10
                  COD       0.90      0.75      0.82        12
           COMPARISON       0.07      0.55      0.13        11
    DELAY_IN_DELIVERY       1.00      0.45      0.62        11
         DISTRIBUTORS       0.00      0.00      0.00        34
                  EMI       0.82      0.36      0.50        25
        ERGO_FEATURES       1.00      0.18      0.31        11
             LEAD_GEN       0.00      0.00      0.00        21
        MATTRESS_COST       0.44      0.55      0.49        22
               OFFERS       0.38      0.80      0.52        10
         ORDER_STATUS       0.80      0.76      0.78        21
       ORTHO_FEATURES       0.75      0.18      0.29        17
              PILLOWS       0.83      1.00      0.91        10
     PRODUCT_VARIANTS       0.30      0.43      0.35        21
      RETURN_EXCHANGE       0.69      0.79      0.73        14
   SIZE_CUSTOMIZATION       0.00      0.00      0.00         9
             WARRANTY       1.00      0.90      0.95        10
   WHAT_SIZE_TO_ORDER       0.73      0.80      0.76        20

             accuracy                           0.46       328
            macro avg       0.60      0.52      0.50       328
         weighted avg       0.55      0.46      0.45       328


Accuracy Score: 0.4573170731707317

DeBERTa V3 Base MNLI Model Metrics:
------------------------

Classification Report:
                       precision    recall  f1-score   support

100_NIGHT_TRIAL_OFFER       1.00      0.44      0.62        18
   ABOUT_SOF_MATTRESS       0.71      0.45      0.56        11
         CANCEL_ORDER       0.83      1.00      0.91        10
        CHECK_PINCODE       1.00      0.10      0.18        10
                  COD       0.35      0.67      0.46        12
           COMPARISON       0.08      0.82      0.15        11
    DELAY_IN_DELIVERY       0.71      0.91      0.80        11
         DISTRIBUTORS       1.00      0.12      0.21        34
                  EMI       1.00      0.48      0.65        25
        ERGO_FEATURES       0.75      0.27      0.40        11
             LEAD_GEN       0.33      0.10      0.15        21
        MATTRESS_COST       0.57      0.36      0.44        22
               OFFERS       0.43      0.90      0.58        10
         ORDER_STATUS       0.71      0.48      0.57        21
       ORTHO_FEATURES       1.00      0.35      0.52        17
              PILLOWS       0.70      0.70      0.70        10
     PRODUCT_VARIANTS       0.30      0.33      0.32        21
      RETURN_EXCHANGE       0.56      0.36      0.43        14
   SIZE_CUSTOMIZATION       0.41      0.78      0.54         9
             WARRANTY       1.00      0.80      0.89        10
   WHAT_SIZE_TO_ORDER       0.67      0.10      0.17        20

             accuracy                           0.43       328
            macro avg       0.67      0.50      0.49       328
         weighted avg       0.70      0.43      0.45       328


Accuracy Score: 0.4298780487804878

Cross Encoder MiniLM Model Metrics:
------------------------

Classification Report:
                       precision    recall  f1-score   support

100_NIGHT_TRIAL_OFFER       1.00      0.39      0.56        18
   ABOUT_SOF_MATTRESS       0.38      0.82      0.51        11
         CANCEL_ORDER       0.00      0.00      0.00        10
        CHECK_PINCODE       1.00      0.20      0.33        10
                  COD       0.82      0.75      0.78        12
           COMPARISON       0.17      0.55      0.26        11
    DELAY_IN_DELIVERY       0.00      0.00      0.00        11
         DISTRIBUTORS       0.27      0.12      0.16        34
                  EMI       1.00      0.48      0.65        25
        ERGO_FEATURES       1.00      0.36      0.53        11
             LEAD_GEN       0.00      0.00      0.00        21
        MATTRESS_COST       0.00      0.00      0.00        22
               OFFERS       0.18      1.00      0.30        10
         ORDER_STATUS       1.00      0.48      0.65        21
       ORTHO_FEATURES       0.47      0.53      0.50        17
              PILLOWS       1.00      0.80      0.89        10
     PRODUCT_VARIANTS       0.21      0.62      0.32        21
      RETURN_EXCHANGE       0.00      0.00      0.00        14
   SIZE_CUSTOMIZATION       0.67      0.22      0.33         9
             WARRANTY       0.23      1.00      0.38        10
   WHAT_SIZE_TO_ORDER       0.65      0.55      0.59        20

             accuracy                           0.38       328
            macro avg       0.48      0.42      0.37       328
         weighted avg       0.47      0.38      0.36       328


Accuracy Score: 0.38414634146341464

StaticLabelsEmbeddingClassifier Model Metrics:
---------------------------------------------
                       precision    recall  f1-score   support

100_NIGHT_TRIAL_OFFER       0.75      0.83      0.79        18
   ABOUT_SOF_MATTRESS       0.48      0.91      0.62        11
         CANCEL_ORDER       0.59      1.00      0.74        10
        CHECK_PINCODE       0.89      0.80      0.84        10
                  COD       1.00      0.67      0.80        12
           COMPARISON       0.50      0.27      0.35        11
    DELAY_IN_DELIVERY       0.60      0.55      0.57        11
         DISTRIBUTORS       1.00      0.62      0.76        34
                  EMI       0.93      0.56      0.70        25
        ERGO_FEATURES       0.78      0.64      0.70        11
             LEAD_GEN       0.00      0.00      0.00        21
        MATTRESS_COST       0.40      0.86      0.54        22
               OFFERS       0.29      1.00      0.45        10
         ORDER_STATUS       0.77      0.95      0.85        21
       ORTHO_FEATURES       0.80      0.24      0.36        17
              PILLOWS       0.53      1.00      0.69        10
     PRODUCT_VARIANTS       0.70      0.33      0.45        21
      RETURN_EXCHANGE       0.53      0.57      0.55        14
   SIZE_CUSTOMIZATION       0.50      0.56      0.53         9
             WARRANTY       0.90      0.90      0.90        10
   WHAT_SIZE_TO_ORDER       0.93      0.65      0.76        20

             accuracy                           0.63       328
            macro avg       0.66      0.66      0.62       328
         weighted avg       0.68      0.63      0.61       328

Accuracy: 0.6310975609756098

GPT 4.1-nano (Prompt #1) Model Metrics:
-------------------------------------
                       precision    recall  f1-score   support

100_NIGHT_TRIAL_OFFER       1.00      0.89      0.94        18
   ABOUT_SOF_MATTRESS       0.73      1.00      0.85        11
         CANCEL_ORDER       1.00      1.00      1.00        10
        CHECK_PINCODE       0.90      0.90      0.90        10
                  COD       1.00      0.92      0.96        12
           COMPARISON       0.90      0.82      0.86        11
    DELAY_IN_DELIVERY       0.86      0.55      0.67        11
    DELIVERY_IN_DELAY       0.00      0.00      0.00         0
         DISTRIBUTORS       1.00      0.85      0.92        34
                  EMI       1.00      0.88      0.94        25
        ERGO_FEATURES       1.00      0.55      0.71        11
             LEAD_GEN       0.72      1.00      0.84        21
        MATTRESS_COST       0.91      0.95      0.93        22
               OFFERS       0.91      1.00      0.95        10
         ORDER_STATUS       0.84      1.00      0.91        21
       ORTHO_FEATURES       0.64      0.94      0.76        17
              PILLOWS       1.00      1.00      1.00        10
     PRODUCT_VARIANTS       0.92      0.52      0.67        21
      RETURN_EXCHANGE       0.93      1.00      0.97        14
   SIZE_CUSTOMIZATION       0.64      1.00      0.78         9
             WARRANTY       1.00      1.00      1.00        10
   WHAT_SIZE_TO_ORDER       0.88      0.75      0.81        20

             accuracy                           0.88       328
            macro avg       0.85      0.84      0.83       328
         weighted avg       0.90      0.88      0.87       328

Accuracy: 0.875

GPT 4.1 (Prompt #1) Model Metrics:
-------------------------------------
                       precision    recall  f1-score   support

100_NIGHT_TRIAL_OFFER       1.00      0.89      0.94        18
   ABOUT_SOF_MATTRESS       0.56      0.82      0.67        11
         CANCEL_ORDER       1.00      1.00      1.00        10
        CHECK_PINCODE       1.00      1.00      1.00        10
                  COD       1.00      1.00      1.00        12
           COMPARISON       0.71      0.91      0.80        11
    DELAY_IN_DELIVERY       0.92      1.00      0.96        11
         DISTRIBUTORS       1.00      0.94      0.97        34
                  EMI       1.00      1.00      1.00        25
        ERGO_FEATURES       1.00      0.82      0.90        11
             LEAD_GEN       0.95      1.00      0.98        21
        MATTRESS_COST       0.91      0.95      0.93        22
               OFFERS       0.91      1.00      0.95        10
         ORDER_STATUS       1.00      0.95      0.98        21
       ORTHO_FEATURES       0.80      0.94      0.86        17
              PILLOWS       1.00      1.00      1.00        10
     PRODUCT_VARIANTS       0.71      0.57      0.63        21
      RETURN_EXCHANGE       0.93      1.00      0.97        14
   SIZE_CUSTOMIZATION       0.69      1.00      0.82         9
             WARRANTY       1.00      1.00      1.00        10
   WHAT_SIZE_TO_ORDER       1.00      0.55      0.71        20

             accuracy                           0.91       328
            macro avg       0.91      0.92      0.91       328
         weighted avg       0.92      0.91      0.91       328

Accuracy: 0.9085365853658537


GPT 4.1.nano (Prompt #2) Model Metrics:
-------------------------------------
                         precision    recall  f1-score   support

- 100_NIGHT_TRIAL_OFFER       0.00      0.00      0.00         0
  100_NIGHT_TRIAL_OFFER       1.00      0.67      0.80        18
     ABOUT_SOF_MATTRESS       0.73      0.73      0.73        11
           CANCEL_ORDER       1.00      1.00      1.00        10
          CHECK_PINCODE       0.53      0.80      0.64        10
                    COD       1.00      0.92      0.96        12
             COMPARISON       0.58      0.64      0.61        11
      DELAY_IN_DELIVERY       1.00      0.09      0.17        11
               DELIVERY       0.00      0.00      0.00         0
   DELIVERY_IN_DELIVERY       0.00      0.00      0.00         0
           DISTRIBUTORS       0.84      0.76      0.80        34
                    EMI       1.00      0.60      0.75        25
          ERGO_FEATURES       1.00      0.27      0.43        11
               LEAD_GEN       0.55      0.57      0.56        21
          MATTRESS_COST       1.00      0.77      0.87        22
           MEASUREMENTS       0.00      0.00      0.00         0
                 OFFERS       0.91      1.00      0.95        10
           ORDER_STATUS       0.73      0.90      0.81        21
            ORIENTATION       0.00      0.00      0.00         0
         ORTHO_FEATURES       0.53      1.00      0.69        17
                PILLOWS       1.00      1.00      1.00        10
            PLACE_ORDER       0.00      0.00      0.00         0
       PRICE_COMPARISON       0.00      0.00      0.00         0
       PRODUCT_VARIANTS       1.00      0.33      0.50        21
        RETURN_EXCHANGE       0.93      1.00      0.97        14
     SIZE_CUSTOMIZATION       0.56      1.00      0.72         9
             WARM_DRINK       0.00      0.00      0.00         0
               WARRANTY       0.91      1.00      0.95        10
     WHAT_SIZE_TO_ORDER       0.92      0.60      0.73        20

               accuracy                           0.73       328
              macro avg       0.61      0.54      0.54       328
           weighted avg       0.85      0.73      0.74       328

Accuracy: 0.725609756097561


GPT-4.1 Model Metrics (Prompt #2):
-------------------------------------
                       precision    recall  f1-score   support

100_NIGHT_TRIAL_OFFER       1.00      0.89      0.94        18
   ABOUT_SOF_MATTRESS       0.60      0.82      0.69        11
         CANCEL_ORDER       1.00      1.00      1.00        10
        CHECK_PINCODE       0.91      1.00      0.95        10
                  COD       1.00      0.92      0.96        12
           COMPARISON       0.67      0.91      0.77        11
    DELAY_IN_DELIVERY       1.00      0.82      0.90        11
         DISTRIBUTORS       1.00      0.88      0.94        34
                  EMI       1.00      1.00      1.00        25
        ERGO_FEATURES       1.00      0.82      0.90        11
             LEAD_GEN       0.73      0.76      0.74        21
        MATTRESS_COST       0.95      0.91      0.93        22
               OFFERS       0.91      1.00      0.95        10
         ORDER_STATUS       0.91      0.95      0.93        21
       ORTHO_FEATURES       0.76      0.94      0.84        17
              PILLOWS       1.00      1.00      1.00        10
          PLACE_ORDER       0.00      0.00      0.00         0
     PRODUCT_VARIANTS       0.60      0.43      0.50        21
      RETURN_EXCHANGE       0.93      1.00      0.97        14
   SIZE_CUSTOMIZATION       0.73      0.89      0.80         9
             WARRANTY       1.00      1.00      1.00        10
   WHAT_SIZE_TO_ORDER       1.00      0.55      0.71        20

             accuracy                           0.86       328
            macro avg       0.85      0.84      0.84       328
         weighted avg       0.90      0.86      0.87       328

Accuracy: 0.8628048780487805