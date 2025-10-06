# Prédiction des Annulations de Réservations - INN Hotels

## Contexte
Les hôtels subissent un **nombre élevé d’annulations de réservations**, souvent dues à des changements de plans ou des conflits d’horaires. Ces annulations sont facilitées par des politiques de **cancellation gratuite ou à faible coût**, ce qui avantage les clients mais réduit les revenus de l’hôtel, surtout pour les **annulations de dernière minute**.  

Avec l’essor des **réservations en ligne**, le comportement des clients et les canaux de réservation ont changé, rendant la **gestion des annulations plus complexe**.

## Objectifs
Ce projet vise à :  
- Identifier les **facteurs influençant les annulations**.  
- Construire un **modèle prédictif** capable d’anticiper les annulations.    

## Description des données
Les données contiennent des informations sur les réservations et les clients. La variable cible est **`booking_status`** (annulée ou non).  

| Colonne | Description |
|---------|------------|
| Booking_ID | Identifiant unique de la réservation |
| no_of_adults / no_of_children | Nombre d’adultes et d’enfants |
| no_of_weekend_nights / no_of_week_nights | Durée du séjour (week-end et semaine) |
| type_of_meal_plan | Plan de repas réservé (Petit-déjeuner, Demi-pension, Pension complète) |
| required_car_parking_space | Besoin de parking (0 = Non, 1 = Oui) |
| room_type_reserved | Type de chambre réservé |
| lead_time | Nombre de jours entre la réservation et l’arrivée |
| arrival_year / arrival_month / arrival_date | Date d’arrivée |
| market_segment_type | Segment de marché du client |
| repeated_guest | Client régulier (0 = Non, 1 = Oui) |
| no_of_previous_cancellations | Nombre d’annulations passées du client |
| no_of_previous_bookings_not_canceled | Réservations passées non annulées |
| avg_price_per_room | Prix moyen par nuit (en €) |
| no_of_special_requests | Nombre de demandes spéciales du client |
| booking_status | Statut de la réservation (annulée ou non) |

## Approche / Méthodologie
1. **Analyse exploratoire des données (EDA)** pour identifier les facteurs influents.  
2. **Prétraitement des données** pour les rendre exploitables par les modèles de Machine Learning.  
3. **Construction et évaluation de modèles prédictifs** pour détecter les annulations.  
4. **Fine-tuning des hyperparamètres** pour optimiser les performances des modèles.  

## Résultats attendus
- Un modèle capable de prédire les annulations de réservations avec précision.  
- Visualisations et analyses des facteurs influençant les annulations.  
