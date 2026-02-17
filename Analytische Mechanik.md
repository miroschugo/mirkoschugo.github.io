- # Lagrange Mechanik
    - ## Zwangsbedingungen
        - Ein $N$-Teilchen System hat im Allgemeinen $3N$ Freiheitsgrade
        - Ist es möglich $p$ Zwangsbedingungen zu finden, so reduziert sich die Anzahl der Freizeitgrade zu $S= 3N - p$
        - ###### Definition 1.1.1
            - **Zwangsbedingungen**↔Bedingungen, die die freie Bewegung der Systemteilchen einschränken
            - **Zwangskräfte**↔Kräfte, die die Zwangsbedingungen bewirken, also freie Teilchenbewegung behindern 
        - ### Holonome Zwangsbedingungen
            - Definition→Verknüpfungen der Teilchenkoordinaten und eventuell der Zeit der Form:

              $$f_v (\boldsymbol r_1, \boldsymbol r_2, \dots, \boldsymbol r_N, t) = 0\,, \qquad v=1,2,\dots,p$$

              
            - #### Holonom-skleronome Zwangsbedingungen
                - Definition→Holonome Zwangsbedingungen, ohne Zeitabhängigkeit:

                  $$\frac{\partial f_v}{\partial t} = 0\,, \qquad v = 1, \dots, p$$

                  
                - Beispiel >>>
                    - Hantel: ![](https://remnote-user-data.s3.amazonaws.com/6X9yYbxj3SHoGxddgUd7BDl-KO72fv8K6ArBFi8bhY_kd1gcHM5pxOoa8Z2_WHE5IhsBDfAIPprXhjj97mYotT9zWcmnvuFB3Je5RmMKr_MXZ41UYStdvvplLl1b01fj.png)
                    - 

                      $$(x_1-x_2)^2+(y_1-y_2)^2+(z_1-z_2)^2 ) = l^2$$

                      
            - #### Holonom-rheonome Zwangsbedingungen
                - Definition→Holonome Zwangsbedingungen, mit expliziter Zeitabhängigkeit:

                  $$\frac{\partial f_v}{\partial t} \neq 0$$

                  
                - Beispiel >>>
                    - Aufzug: ![](https://remnote-user-data.s3.amazonaws.com/V3X7JtuqwTUcR1Zm3RPgmVem_5PmPpH6YPYocLeY320vVkkg8VeB7hnvdFaaV4jwYai7pmYz63SZwbpNei9eN2la9FK98ssgxv4fWD_AGQfwsXQD50qFQPFLfNiCSZqw.png)
                    - 

                      $$z(t) = v_0\,(t-t_0)+z_0$$

                      
        - ### Nicht-holonome Zwangsbedingungen
            - Definition→Sind Zwangsbedingungen, die sich nicht wie

              $$f_v (\boldsymbol r_1, \boldsymbol r_2, \dots, \boldsymbol r_N, t) = 0$$

              darstellen lassen
            - #### Ungleichungen
                - Beispiel→

                  $$(x^2 + y^2 + z^2 )- R^2 \ge 0$$

                  
            - #### Differentielle, nicht integrierbare Formen
                - 

                  $$\sum_{m=1}^{3N} f_{im} \mathrm dx_m + f_{it} \mathrm dt = 0, \quad i = 1, \dots, p$$

                  [2) Zwangsbedingungen in differentieller, nicht integrierbarer Form](Analytische%20Mechanik/Grundkurs%20Theoretische%20Physik%202%20-%20Analytische%20Mechanik/Highlights/Page%20024/2)%20Zwangsbedingungen%20in%20differentieller%2C%20nicht%20integrierbarer%20Form.md)
                    - Falls es kein

                      $$f_{im} = \frac{\partial F_i}{\partial x_m}, \quad \forall \, m\,; \quad \frac{\partial F_i}{\partial t} = f_{it}$$

                      
gibt
                    - Existiere hingegen $F_i$, wäre ja

                      $$\mathrm dF = \sum_{m=1}^{3N} \frac{\partial F_i}{\partial x_m} \mathrm dx_m + \frac{\partial F_i}{\partial t}\mathrm dt = 0$$

                      
das totale Differential ⇒ die Gleichung integrierbar
    - ## Generalisierte Koordinaten
        - System mit $S=3N-p$ Freiheitsgraden ⇒ $p$ kartesische Koordinaten eliminieren, Newton lösen ⇒ unelegant
        - ###### Generalisierte Koordinaten

          $$q_1, q_2, \dots, q_S$$

          
            - Bedingungen >>>
                - Eindeutigkeit ⇔ es gelte die Transformationsformel

                  $$\bm r_i = \bm r_i \,(q_1, \dots, q_s,t)\, , \qquad i = 1,2,\dots,N$$

                  
                - Unabhängigkeit ⇔ es gibt keine Beziehung der Form 

                  $$f(q_1, \dots, q_S,t) = 0$$

                  
        - ###### Konfigurationsraum
            - ###### Definition→$S$-dimensionaler Raum, der durch die generalisierten Koordinaten aufgespannt wird
            - ###### 

              $$\bm q = (q_1, q_2, \dots, q_S)$$

               nennt man einen {{Konfigurationsvektor }} 
            - ###### 

              $$\dot q_1, \dot q_2, \dots, \dot q_S$$

              
nennt man generalisierte {{Geschwindigkeiten}}
            - 
    - ## d'Alembert Prinzip
        - ### Treibende Kräfte und Zwangskräfte
            - $\boldsymbol F_i$ ist die auf das Teilchen $i$ wirkende Kraft

              $$\boldsymbol F_i = \boldsymbol K_i + \boldsymbol Z_i = m_i \ddot {\boldsymbol r}_i$$

              
            - Dabei handelt es sich bei $\boldsymbol Z_i$ um die Zwangskraft auf Teilchen $i$

            - 
        - ### Prinzip der Virtuellen Arbeit 
            - Multipliziert man diese Kraft mit $\delta \boldsymbol r$ ([Virtuelle Verrückung](../../Virtual%20Displacements.md)), so erhält man die virtuelle Arbeit
            - ###### Definition 1.2.2  *Virtuelle Arbeit*  

              $$\delta W_i = - \boldsymbol F_i \cdot \delta \boldsymbol r_i$$

              
            - ###### Prinzip der virtuellen Arbeit

              $$\sum_i \boldsymbol Z_i \cdot \delta \boldsymbol r_i = 0$$

                  
                - Die gedachten Bewegungen unter der Zwangskraft leisten keine Arbeit
                - Nicht mathematisch abgeleitet ⇒ Erfahrungstatsache
            - Aus [1.19](Analytische%20Mechanik/Lagrange%20Mechanik/d'Alembert%20Prinzip/Prinzip%20der%20Virtuellen%20Arbeit/Prinzip%20der%20virtuellen%20Arbeit_sum_i%20_boldsymbol%20Z_i%20_cdot%20_delta%20_boldsymbol%20r_i%20%3D%200.md) und [1.17](Analytische%20Mechanik/Lagrange%20Mechanik/d'Alembert%20Prinzip/Treibende%20Kr%C3%A4fte%20und%20Zwangskr%C3%A4fte/_boldsymbol%20F_i%20ist%20die%20auf%20das%20Teilchen%20i%20wirkende%20Kraft_boldsymbol%20F_i%20%3D%20_boldsymbol%20K_i%20%2B%20_boldsymbol%20Z_i%20%3D%20m_i%20_ddot%20%7B_boldsymbol%20r%7D_i.md) folgt
                - ###### d'Alembert'sches Prinzip 

                  $$\sum_{i=1}^N (\boldsymbol K_i - m_i \ddot {\boldsymbol r}_i) \cdot \delta \boldsymbol r_i = 0$$

                  
        - ### Erweitertes d'Alembert Prinzip
            - Transformationsformel

              $${\boldsymbol r}_i = {\boldsymbol r}_i(q_1, q_2, \ldots, q_S, t), \quad i = 1,2,\ldots, N$$

               
            - Mit [1.21](Analytische%20Mechanik/Lagrange%20Mechanik/d'Alembert%20Prinzip/Erweitertes%20d'Alembert%20Prinzip/Transformationsformel%7B_boldsymbol%20r%7D_i%20%3D%20%7B_boldsymbol%20r%7D_i(q_1%2C%20q_2%2C%20_ldots%2C%20q_S%2C%20t)%2C%20_quad%20i%20%3D%201%2C2%2C_ldots%2C%20N.md) ergibt sich

              $$\dot {\bm r}_i = \sum_{j=1}^S \frac{\partial \bm r_i}{\partial q_j} \ \dot q_j + \frac{\partial \bm r_i}{\partial t} \\$$

                 
            - Es gilt außerdem

              $$\frac{\partial \boldsymbol r_i}{\partial q_j} = \frac{\partial \dot {\boldsymbol r}_i}{\partial \dot q_j}$$

              
                - Beweis >>>
                    - --------------------- Portal ---------------------
                        - Studium
                    - --------------------- Portal ---------------------
                        - Studium
                    - 

                      $$\implies \frac{\partial \dot {\bm r}_i}{\partial \dot q_j} = \underbrace{ 
\frac{\partial}{\partial \dot q_j} \sum_{k=1}^S \frac{\partial {\bm r}_i}{\partial q_k} \, \dot q_k}
_{\text{für }k\neq j\, \to \,0} + 


\frac{\partial}{\partial \dot q_i} \, \underbrace{\frac{\partial \bm r_i}{\partial t}}
_{\neq f(\dot q)}

= \frac{\partial {\bm r}_i}{\partial q_j} \quad \blacksquare$$

                       
            - Wegen $\delta t = 0$

              $$\delta \bm r_i = \sum_{j=1}^S \frac{\partial \bm r_i}{\partial q_j} \, \delta q_j$$

              
            - Erster Summand
            - 

              $$\sum_i \boldsymbol K_i \cdot \delta \boldsymbol r_i \stackrel{(A)}{=} \sum_{i=1}^N \boldsymbol K_i \sum_{j=1}^S \frac{\partial \boldsymbol r_i}{\partial q_j} \delta q_j \equiv \sum_{j=1}^S Q_j\delta q_j$$

                  Wobei die $Q_j$ die **generalisierten Kraftkomponenten** heißen
            - ###### Definition 1.2.3  *Generalisierte Kraftkomponenten*  

              $$Q_j = \sum_{i=1}^N \bm K_i \cdot \frac{\partial \bm r_i}{\partial q_j}$$

              
            - Zweiter Summand
            - 

              $$\begin{align*}
\sum_{i=1}^N m_i \ddot{\bm r}_i \cdot \delta \bm r_i
&= {{c1::\sum_{i=1}^N \sum_{j=1}^S m_i \ddot{\bm r}_i \cdot
\frac{\partial \bm r_i}{\partial q_j} \, \delta q_j}} \\

&= {{c1::  \sum_{i=1}^N \sum_{j=1}^S m_i \left\{ \frac{d}{d t} \left( \dot{\bm r}_i  \cdot
\frac{\partial \bm r_i}{\partial q_j}  \right)  -  \dot{\bm r}_i \frac{d}{d t} \frac{\partial \bm r_i}{\partial q_j} \right\} \, \delta q_j
}} \\

&=  {{c1::\sum_{i=1}^N \sum_{j=1}^S m_i \left\{ \frac{d}{d t} \left( \dot{\bm r}_i  \cdot
\frac{\partial \dot{\bm r}_i}{\partial \dot q_j}  \right)  -  \dot{\bm r}_i \cdot \frac{\partial \dot {\bm r}_i}{\partial q_j} \right\} \, \delta q_j \tag{*} }}\\

&=  {{c1::\sum_{i=1}^N \sum_{j=1}^S m_i \left\{ \frac{d}{d t} \left[ \frac{\partial}{\partial \dot q_j}  \left( \frac{1}{2}\dot{\bm r}_i^2 \right) \right]  -  \frac{\partial}{\partial \dot q_j} \left( \frac{1}{2}\dot{\bm r}_i^2 \right) \right\} \, \delta q_j}} \\

&=  \sum_{j=1}^S  \left\{ \frac{d}{d t} \left( \frac{\partial T}{\partial \dot q_j} \right)  -  \frac{\partial T}{\partial \dot q_j} \right\} \, \delta q_j \\

\end{align*}$$

              
            - $(*)$ ist keines Falls selbstverständlich. Zum einen wurde [1.23](Analytische%20Mechanik/Lagrange%20Mechanik/d'Alembert%20Prinzip/Erweitertes%20d'Alembert%20Prinzip/Es%20gilt%20au%C3%9Ferdem_frac%7B_partial%20_boldsymbol%20r_i%7D%7B_partial%20q_j%7D%20%3D%20_frac%7B_partial%20_dot%20%7B_boldsymbol%20r%7D_i%7D%7B_partial%20_dot%20q_j%7D.md) benutzt. Ferner wurde benutzt:

              $$\begin{align*}
    
\frac{d}{d t} \frac{\partial \boldsymbol r_i}{\partial q_j} &= 

{{c1::\sum_{l=1}^S \frac{\partial^2 \boldsymbol r_i}{\partial q_l \, \partial q_j} \dot q_l + \frac{\partial ^2 \boldsymbol r_i}{\partial t \, \partial q_j}}} \\
    
&= {{c1::\frac{ \partial}{ \partial q_j}  \left\{  \sum_{l=1}^S \frac{\partial \boldsymbol r_i}{\partial q_l} \dot q_l + \frac{\partial \boldsymbol r_i}{\partial t} \right\}}}

= {{c1::\frac{\partial }{\partial q_j} \left\{ \dot{\boldsymbol r_i}  \right\} }}

= \frac{\partial \dot{\boldsymbol r}_i}{\partial q_j}

\end{align*}$$

              
            - Setzt man nun die beiden Summanden zusammen, so erhält man das angepasste d'Alembert'sche Prinzip
            1. 

              $$\sum_{j=1}^S \left\{  \left[   \frac{d}{d t} \left( \frac{\partial T}{\partial \dot q_j} \right)  - \frac{\partial T}{\partial q_j} \right] - Q_j \right\} \delta q_j = 0$$

              
            - #### 1) Holonome Zwangsbedingungen
                - Alle $q_j$ unabhängig ⇒ Alle bis auf eines gleich 0
                - ###### d'Alembert für holonome Zwangsbedingungen 

                  $$\frac{\mathrm d}{\mathrm dt}\left( \frac{\partial T}{\partial \dot q_j}\right) - \frac{\partial T}{\partial q_j} = Q_j, \qquad j = 1,2,\dots, S$$

                  
            - #### 2) Konservatives System
                - Nun gilt

                  $$\bm K_i = -\nabla_i V$$

                  
                - Mit ([1.26](Analytische%20Mechanik/Lagrange%20Mechanik/d'Alembert%20Prinzip/Erweitertes%20d'Alembert%20Prinzip/Definition%201.2.3%20Generalisierte%20Kraftkomponenten%20Q_j%20%3D%20_sum_%7Bi%3D1%7D%5EN%20_bm%20K_i%20_cdot%20_frac%7B_partial%20_bm%20r_i%7D%7B_partial%20q_j%7D.md))

                  $$Q_j = \sum_{i=1}^N(-\nabla_iV)\cdot \frac{\partial \bm r_i}{\partial q_j} = -\frac{\partial V}{\partial q_j}$$

                  
                - ###### d'Alembert für konservative Systeme

                  $$\sum_{j=1}^S \left[ \frac{\mathrm d}{\mathrm dt} \frac{\partial}{\partial \dot q_j}( T - V) - \frac{\partial}{\partial q_j} ( T - V) \right] \cdot \delta q_j= 0$$

                  
    - ## Lagrange Gleichung
        - 
        - Für das [d'Alembert Prinzip](Analytische%20Mechanik/Lagrange%20Mechanik/d'Alembert%20Prinzip.md) hatten wir gefunden

          $$\sum_{i=1}^N (\boldsymbol K_i - m_i \ddot {\boldsymbol r}_i) \cdot \delta \boldsymbol r_i = 0 \iff \sum_{j=1}^S \left\{  \left[   \frac{d}{d t} \left( \frac{\partial T}{\partial \dot q_j} \right)  - \frac{\partial T}{\partial q_j} \right] - Q_j \right\} \delta q_j = 0$$

          

        - Für **holonome Zwangsbedigungen** sind die Koordinaten $q_j$ unabhängig voneinander
            - Das bedeutet, wir können alle bis auf eine gleich 0 setzen, was zeigt, dass nicht nur die Summe, sondern gleich jeder Summand verschwindet

              $$\frac{d}{dt} \left( \frac{\partial T}{\partial \dot q_j} \right)  - \frac{\partial T}{\partial q_j}  = Q_j$$

              

        - Für ein **konservatives System** gilt wiederum


          $$Q_j = \sum_{i=1}^N \boldsymbol K_i \cdot \frac{\partial \boldsymbol r_i}{\partial q_j} =\sum_{i=1}^N (-\nabla_i V) \cdot \frac{\partial \boldsymbol r_i}{\partial q_j} = - \frac{\partial V}{\partial q_j}$$

          
            - Hier existiert ein Potenzial

              $$V= V(\bm r_1, \dots, \bm r_N)$$

              
            - Generalisierte Kraftkomponente:

              $$Q_j = \sum_{i=1}^N (-\nabla _i \,V )\cdot \frac{\partial \bm r_i}{\partial q_j} = -\frac{\partial V}{\partial q_j}\,,\qquad j = 1, 2, \dots ,S$$

              
            - Daher dürfen wir $\boldsymbol K_i$ so ausdrücken
            - Also

              $$\sum_{j=1}^S \left[   \frac{d}{d t} \frac{\partial }{\partial \dot q_j} (T-V)  - \frac{\partial }{\partial q_j} (T-V) \right] \delta q_j = 0$$

              

            - ###### Lagrange-Funktion 

              $$L(q_1, \dots, q_S, \dot{q}_1, \dots, \dot{q}_S, t) = T(q_1, \dots, q_S, \dot{q}_1, \dots, \dot{q}_S, t) - V(q_1, \dots, q_S, t)$$

              
            - Und es folgt
            - 

              $$\sum_{j=1}^S \left[     \frac{d}{dt} \frac{\partial L}{\partial \dot q_j} - \frac{\partial L}{\partial q_j}     \right] \cdot \delta q_j = 0$$

              
            - 
        - Der Regelfall von mechanischen Systemen ist ein **konservatives System mit holonomen Zwangsbedingungen:** 
            - ###### Lagrange-Gleichung (2. Art)

              $$\frac{d}{dt} \frac{\partial L}{\partial \dot q_j} - \frac{\partial L}{\partial q_j}   = 0, \qquad j =1,2,\dots, S$$

              
        - ###### Definition 1.2.5  *Verallgemeinerter Impuls*  

          $$p_i = \frac{\partial L}{\partial \dot q_i}$$

          
        - ###### Definition 1.2.6  *Zyklische Koordinate*  

          $$q_j \; \text{zyklisch} \quad \Leftrightarrow \quad \frac{\partial L}{\partial q_j} = 0 \quad \Leftrightarrow \quad p_j = \frac{\partial L}{\partial \dot q_j} = const.$$

          
        - 
    - ## Lagrange Multiplikatoren
        - Für Systeme mit **nicht-holonomen Zwangsbedingungen**
            - --------------------- Portal ---------------------
                - Studium
        - Vergleiche:
            - --------------------- Portal ---------------------
                - Studium
            - --------------------- Portal ---------------------
                - Studium
        - Im Allgemeinen bestehen Systeme aus $\bar p$ holonomen und $p$ nicht-holonomen Zwangsbedingungen
        - Freiheitsgrad

          $$j = 3N - ( \bar p - p)$$

          
            - Vorher: $S = 3N - p$
            - Jetzt: $S = 3N - \overline p = j-p$
        - --------------------- Portal ---------------------
            - Studium
        - Diese sind nicht notwendigerweise unabhängig voneinander $f_{im} = f_{im}(x_1, \dots, x_{3N}, t), \, f_{it} = f_{it}(x_1, \dots, x_{3N}, t)$
            - --------------------- Portal ---------------------
                - Studium
        - Auf $q_j$ umschreiben:

          $$\sum_{m=1}^j a_{im} \, dq_m + b_{it} dt = 0 \implies \sum_{j=1}^j a_{im}\,\dot q_m + b_{it} = 0$$

          
        - Formulierung für $\delta \boldsymbol q$ mit $\delta t = 0$

          $$\sum_{m=1}^j a_{im} \, \delta q_m = 0$$

          
        - Multiplikation mit einem noch ominösen $\lambda$ ⇒ unabhängig, $p$ stück

          $$\sum_{i=1}^p \lambda_i \sum_{m=1}^j a_{im}\, \delta q_m = 0$$

          
        - Für ein konservatives System mit holonomen Zwangsbedingungen hatten wir gefunden
            - --------------------- Portal ---------------------
                - Studium
        - Diese Systeme können wir nun kombinieren:

          $$\sum_{m=1}^j \left\{ \frac{\partial L}{\partial q_m} - \frac{d}{dt} \frac{\partial L}{\partial \dot{q}_m} + \sum_{i=1}p \lambda_i a_{im} \right\} \delta q_m = 0.$$

          
        - Trotzdem sind die $\delta q_m$ nicht unabhängig... 

          $$q_m: \quad m = 1, \dots, j-p \quad (\text{unabhängig})\\q_m: \quad m=j-p+1, \dots, j \quad (\text{abhängig})$$

          
        - Wähle also die  _ ***noch unbestimmten*** _  $\lambda_i$ so, dass

          $$\frac{\partial L}{\partial q_m} - \frac{d}{dt} \frac{\partial L}{\partial \dot{q}_m} + \sum_{i=1}p \lambda_i a_{im} \stackrel{!}{=} 0, \quad m = j-p+1, \dots, j$$

          
            - nun sind die verbleibenden $j-p$ der $\delta q_m$ unabhängig. Somit sind alle $j$ Gleichungen unabhängig
        - ###### Lagrange'sche Bewegungsgleichung (1. Art)

          $$\frac{d}{dt} \frac{\partial L}{\partial \dot{q}_m} - \frac{\partial L}{\partial q_m} = \sum_{i=1}^{p} \lambda_i a_{im}, \quad m = 1, \dots, j$$

          
        - Was ist die physikalische Bedeutung von $\lambda _i$?
            - Vergleiche ([1.102](Analytische%20Mechanik/Lagrange%20Mechanik/Lagrange%20Multiplikatoren/Lagrange'sche%20Bewegungsgleichung%20(1.%20Art)_frac%7Bd%7D%7Bdt%7D%20_frac%7B_partial%20L%7D%7B_partial%20_dot%7Bq%7D_m%7D%20-%20_frac%7B_partial%20L%7D%7B_partial%20q_m%7D%20%3D%20_sum_%7Bi%3D1%7D%5E%7Bp%7D%20_lambda_i%20a_%7Bim%7D%2C%20_quad%20m%20%3D%201%2C%20_dots%2C%20j.md)) mit ([1.33](Analytische%20Mechanik/Lagrange%20Mechanik/d'Alembert%20Prinzip/Erweitertes%20d'Alembert%20Prinzip/1)%20Holonome%20Zwangsbedingungen/d'Alembert%20f%C3%BCr%20holonome%20Zwangsbedingungen%20_frac%7B_mathrm%20d%7D%7B_mathrm%20dt%7D_left(%20_frac%7B_partial%20T%7D%7B_partial%20_dot%20q_j%7D_right)%20-%20_frac%7B_partial%20T%7D%7B_partial%20q_j%7D%20%3D%20Q_j%2C%20_qquad%20j%20%3D%201%2C2%2C_dots%2C%20S.md))

              $$\overline Q_m = \sum_{i=1}^p \lambda_i\,a_{im}$$

              
            - Oder mit ([1.97](Analytische%20Mechanik/Lagrange%20Mechanik/Lagrange%20Multiplikatoren/Multiplikation%20mit%20einem%20noch%20omin%C3%B6sen%20_lambda%20%E2%87%92%20unabh%C3%A4ngig%2C%20p%20st%C3%BCck_sum_%7Bi%3D1%7D%5Ep%20_lambda_i%20_sum_%7Bm%3D1%7D%5Ej%20a_%7Bim%7D_%2C%20_delta%20q_m%20%3D%200.md)) zum **d'Alembert'schen Prinzip für die generalisierte Zwangskraft**

              $$\sum_{m=1}^j \overline Q_m\,\delta q_m = 0$$

              
        - ### Beispiel
            - Atwood'sche Fallmaschine
![](https://remnote-user-data.s3.amazonaws.com/eZozNBULsJ-Dmz5CnNPKwVQcgCuQdbzkt4h46GdQiAt1TObn0_3BWGAuyEF9yb3FFd4ULVnhfmRTyEUgYKnzLLpqSd3ErOFO7sbsyamITqWyRiRu_tjt_KZ2Zp-k8een.png)

            - Eigentlich holonom, aber man kann auch holonome Zwangskräfte als nicht holonome behandeln ⇒ mehr Infos über das system
            - Zwangsbedingungen

              $$y_1 = z_1 = z_2 = 0\,,\quad y_2 = 2R\,,\quad x_1 + x_2 = l - \pi R$$

              
            - Generalisierte Koordinate

              $$q_1 = x_1\,; \quad q_2 = x_2$$

              
            - Nur die ersten vier als holonom betrachtet, die übrige:

              $$f(q_1, q_2, t) = q_1+q_2 - l + \pi R = 0 \implies \mathrm df = \mathrm dq_1 + \mathrm dq_2$$

              
                - Totales Differential
            - Vergleich mit ([1.95](Analytische%20Mechanik/Lagrange%20Mechanik/Lagrange%20Multiplikatoren/Auf%20q_j%20umschreiben__sum_%7Bm%3D1%7D%5Ej%20a_%7Bim%7D%20_%2C%20dq_m%20%2B%20b_%7Bit%7D%20dt%20%3D%200%20_implies%20_sum_%7Bj%3D1%7D%5Ej%20a_%7Bim%7D_%2C_dot%20q_m%20%2B%20b_%7Bit%7D%20%3D%200.md)) ⇒ $a_{11} = a_{12} = 1$
                - Zur Erinnerung $a_{im}$: 
                    - $i = 1,\dots,p$ nicht-holonome Zwangsbedingungen
                    - $m = 1,\dots, j$: holonome Zwangsbedingungen
                    - mit $j = 3N-(\overline p-p), \quad p\le\overline p$
                    - $\overline p$: Gesamtzahl der Zwangsbedingungen (holonom + nicht holonom)
            - ([1.104](Analytische%20Mechanik/Lagrange%20Mechanik/Lagrange%20Multiplikatoren/Was%20ist%20die%20physikalische%20Bedeutung%20von%20_lambda%20_i_/Vergleiche%20(1.102)%20mit%20(1.33)_overline%20Q_m%20%3D%20_sum_%7Bi%3D1%7D%5Ep%20_lambda_i_%2Ca_%7Bim%7D.md)) zeigt ⇒ $\overline Q_1 = \overline Q_2 = \lambda$
            - Leite ([1.95](Analytische%20Mechanik/Lagrange%20Mechanik/Lagrange%20Multiplikatoren/Auf%20q_j%20umschreiben__sum_%7Bm%3D1%7D%5Ej%20a_%7Bim%7D%20_%2C%20dq_m%20%2B%20b_%7Bit%7D%20dt%20%3D%200%20_implies%20_sum_%7Bj%3D1%7D%5Ej%20a_%7Bim%7D_%2C_dot%20q_m%20%2B%20b_%7Bit%7D%20%3D%200.md)) nach der Zeit ab und setze Zwangsbedingungen ein

              $$\dot q_1 + \dot q_2 = 0$$

              
            - 
        - In holonomen Systemen gehen Informationen über Zwangskräfte verloren
            - Betrachte $N$-Teilchen System mit $p$ holonomen Zwangsbedingungen

              $$f_v (\bm r_1,\dots, \bm r_N,t) = 0\,,\quad v = 1,\dots, p$$

              
            - Keine [Verringerung der Freiheitsgrade](Analytische%20Mechanik/Grundkurs%20Theoretische%20Physik%202%20-%20Analytische%20Mechanik/Highlights/Page%20055/Verringerung%20der%20Variablenzahl.md) ⇒ [Teilchenorte direkt als „generalisierte“ Koordinaten](Analytische%20Mechanik/Grundkurs%20Theoretische%20Physik%202%20-%20Analytische%20Mechanik/Highlights/Page%20055/Teilchenorte%20direkt%20als%20%E2%80%9Egeneralisierte%E2%80%9C%20Koordinaten.md) verwenden 

              $$\bm r_i = (x_{i1},\, x_{i2},\, x_{i3})$$

              
            - Aus den Zwangsbedingungen folgt

              $$\mathrm df_v = \sum_{i=1}^N\sum_{j=1}^3\frac{\partial f_v}{\partial x_{ij}} \mathrm d x_{ij} + \frac{\partial f_v}{\partial t}\mathrm dt = \sum_{i=1}^N \nabla_if_v\cdot \mathrm d\bm r_i + \frac{\partial f_v}{\partial t}\mathrm dt \\
\ \\

\curvearrowright \sum_{i=1}^N \dot{\bm r} \cdot \nabla_if_v = - \frac{\partial f_v}{\partial t}\mathrm dt$$

              
                - Hier ist 

                  $$\nabla_i = \left( \frac{\partial}{\partial x_{i1}},\,\frac{\partial}{\partial x_{i2}},\,\frac{\partial}{\partial x_{i3}} \right)$$

                  
                - und das Skalarprodukt

                  $$\sum_{j=1}^3 a_ib_i = \bm a\cdot \bm b$$

                  
            - Virtuelle Verrückung + $\delta t = 0$

              $$\sum_{i=1}^N \nabla_if_v \cdot \delta \bm r_i = 0$$

              
            - Nutze ([1.20](Analytische%20Mechanik/Lagrange%20Mechanik/d'Alembert%20Prinzip/Prinzip%20der%20Virtuellen%20Arbeit/Aus%201.19%20und%201.17%20folgt/d'Alembert'sches%20Prinzip%20_sum_%7Bi%3D1%7D%5EN%20(_boldsymbol%20K_i%20-%20m_i%20_ddot%20%7B_boldsymbol%20r%7D_i)%20_cdot%20_delta%20_boldsymbol%20r_i%20%3D%200.md)) und addiere die Nullgleichung, offensichtlich bleibt der Wert 0 nach Multiplikation mit $\lambda_v$

              $$\sum_{i=1}^N \left( \boldsymbol K_i - m_i \ddot {\boldsymbol r}_i +\sum_{v=1}^p \lambda_v \nabla_if_v \right) \cdot \delta \boldsymbol r_i = 0$$

              
                - Es müssen $p$-Stück sein, da die $\delta r_i$ sicher nicht alle unabhängig sind ("normale Koordinaten)
            - Wähle $\lambda_v$ so, dass die Bestimmungsgleichung gleich 0 wird 

              $$m_i\ddot{\bm r}_i = \bm K_i + \sum_{v=1}^p\lambda_v\nabla_if_v \implies \bm Z_i = \sum_{v=1}^p\lambda_v\nabla_if_v$$

              
                - Vergleiche ([1.17](Analytische%20Mechanik/Lagrange%20Mechanik/d'Alembert%20Prinzip/Treibende%20Kr%C3%A4fte%20und%20Zwangskr%C3%A4fte/_boldsymbol%20F_i%20ist%20die%20auf%20das%20Teilchen%20i%20wirkende%20Kraft_boldsymbol%20F_i%20%3D%20_boldsymbol%20K_i%20%2B%20_boldsymbol%20Z_i%20%3D%20m_i%20_ddot%20%7B_boldsymbol%20r%7D_i.md))
    - ## Hamilton Prinzip
        - ### Formulierung des Prinzips
            - --------------------- Portal ---------------------
                - Konfigurationsraum::Der $S$-dimensionale Raum, dessen Achsen durch die generalisierten Koordinaten $q_1, \dots, q_S$ gebildet werden.[▸ Konﬁgurationsraum verstehen wir den S-dimensionalen Raum, dessen Achsen durch die generalisierten Koordinaten q1 , . . . , q S gebildet werden.](Analytische%20Mechanik/Grundkurs%20Theoretische%20Physik%202%20-%20Analytische%20Mechanik/Highlights/Page%20079/%E2%96%B8%20Kon%EF%AC%81gurationsraum%20verstehen%20wir%20den%20S-dimensionalen%20Raum%2C%20dessen%20Achsen%20durch%20die%20generalisierten%20Koordinaten%20q1%20%2C%20.%20.%20.%20%2C%20q%20S%20gebildet%20werden.md)
            - [Abb. 1.43 Eindimensionale Veranschaulichung der in Deﬁnition 1.3.1 eingeführten Konkurrenzschar von Konﬁgurationsbahnen](Analytische%20Mechanik/Grundkurs%20Theoretische%20Physik%202%20-%20Analytische%20Mechanik/Highlights/Page%20080/Abb.%201.43%20Eindimensionale%20Veranschaulichung%20der%20in%20De%EF%AC%81nition%201.3.1%20eingef%C3%BChrten%20Konkurrenzschar%20von%20Kon%EF%AC%81gurationsbahnen.md)
![](https://remnote-user-data.s3.amazonaws.com/jtMWLqwnyzu77Qd586uogvSxTkbwUKKd0zjVWnS93Oroy6yKNaFV0tu8MAoqGmc4TIBIQfZ8JcDiWTpmcDFyHhdB2eLIEac-RmZ5czQ9NE2gT6ysRgvC-jQT-vRvgZKB.png)
            - Wir deﬁnieren: 

              $$S \{q(t)\} = {{c1::\int_{t_1}^{t_2} \widetilde L (t) \ \mathrm dt}}$$

              [Wir deﬁnieren: S {q(t)} = t2 ∫ t1̃ L(t) dt .](Analytische%20Mechanik/Grundkurs%20Theoretische%20Physik%202%20-%20Analytische%20Mechanik/Highlights/Page%20080/Wir%20de%EF%AC%81nieren_%20S%20%7Bq(t)%7D%20%3D%20t2%20%E2%88%AB%20t1%CC%83%20L(t)%20dt%20.md)
            - [Deﬁnition 1.3.1](Analytische%20Mechanik/Grundkurs%20Theoretische%20Physik%202%20-%20Analytische%20Mechanik/Highlights/Page%20080/De%EF%AC%81nition%201.3.1.md)
                - $M \equiv \left\{ \bm q (t) : \bm q(t_1) = \bm q_a \; ; \quad \bm q(t_2) = \bm q_e \right\}$
                    - Eigenschaften >>>
                        - [1. Gleiche Endpunktzeiten t1 , t2 , d. h. gleiche „Durchlaufzeiten“ für das System.](Analytische%20Mechanik/Grundkurs%20Theoretische%20Physik%202%20-%20Analytische%20Mechanik/Highlights/Page%20080/1.%20Gleiche%20Endpunktzeiten%20t1%20%2C%20t2%20%2C%20d.%20h.%20gleiche%20%E2%80%9EDurchlaufzeiten%E2%80%9C%20f%C3%BCr%20das%20System.md)
                        - [2. Jede Bahn ist durch virtuelle Verrückungen aus der tatsächlichen Bahn entstanden.](Analytische%20Mechanik/Grundkurs%20Theoretische%20Physik%202%20-%20Analytische%20Mechanik/Highlights/Page%20080/2.%20Jede%20Bahn%20ist%20durch%20virtuelle%20Verr%C3%BCckungen%20aus%20der%20tats%C3%A4chlichen%20Bahn%20entstanden.md)
                        - [3. Die virtuellen Verrückungen der Endpunkte qa , qe sind für alle Bahnen Null:](Analytische%20Mechanik/Grundkurs%20Theoretische%20Physik%202%20-%20Analytische%20Mechanik/Highlights/Page%20080/3.%20Die%20virtuellen%20Verr%C3%BCckungen%20der%20Endpunkte%20qa%20%2C%20qe%20sind%20f%C3%BCr%20alle%20Bahnen%20Null_.md)

                          $$\delta \bm q_a = \delta \bm q_e = 0$$

                          
            - ###### **Wirkungsfunktional**

              $$S\{ \bm q (t) \} = \int_{t_1} ^{t_2} L(\bm q(t), \, \dot{\bm q}(t), \, t) \, \mathrm dt$$

              
            - ###### Hamilton'sches Prinzip
                - [A) Die Systembewegung erfolgt so, dass S{q(t)} auf der in (1.118) deﬁnierten Konkurrenzschar M für die tatsächliche Bahn extremal („stationär“) wird.](Analytische%20Mechanik/Grundkurs%20Theoretische%20Physik%202%20-%20Analytische%20Mechanik/Highlights/Page%20081/A)%20Die%20Systembewegung%20erfolgt%20so%2C%20dass%20S%7Bq(t)%7D%20auf%20der%20in%20(1.118)%20de%EF%AC%81nierten%20Konkurrenzschar%20M%20f%C3%BCr%20die%20tats%C3%A4chliche%20Bahn%20extremal%20(%E2%80%9Estation%C3%A4r%E2%80%9C)%20wird.md)
                - [B) Die Systembewegung erfolgt so, dass die Variation von S auf M bezüglich der tatsächlichen Bahn q(t) verschwindet:](Analytische%20Mechanik/Grundkurs%20Theoretische%20Physik%202%20-%20Analytische%20Mechanik/Highlights/Page%20081/B)%20Die%20Systembewegung%20erfolgt%20so%2C%20dass%20die%20Variation%20von%20S%20auf%20M%20bez%C3%BCglich%20der%20tats%C3%A4chlichen%20Bahn%20q(t)%20verschwindet_.md)

                  $$\delta S = \delta \! \int_{t_1}^{t_2} L(\bm q(t), \, \dot{\bm q}(t), \, t) \, \mathrm dt \stackrel{!}{=} 0.$$

                  
            - ###### Äquivalenz zum [d'Alembert Prinzip](Analytische%20Mechanik/Lagrange%20Mechanik/d'Alembert%20Prinzip.md)
                - --------------------- Portal ---------------------
                    - Studium
                - [Virtuelle Verrückung](../../Virtual%20Displacements.md) $\delta  \bm r$ sind differenzierbare Zeitfunktionen:

                  $$\ddot {\bm r}_i \cdot \delta \bm r_i = \frac{\mathrm d}{\mathrm dt} \, (\dot{\bm r}\cdot \delta \bm r_i) - \dot {\bm r}_i \cdot \delta \dot {\bm r}_i = \frac{\mathrm d}{\mathrm dt} \, (\dot {r}_i\cdot \delta \bm r_i ) - \frac{1}{2} \, \delta \left( \dot{\bm r}_i^2 \right)$$

                  
                - Integriere $(1.20)$ zwischen $t_1$ und $t_2$: 

                  $$\int_{t_1}^{t_2} \left( \sum_{i=1}^N (m_i\,\bm{\ddot r}_i  - \bm K_i ) \cdot \delta \boldsymbol r_i \right) \, \mathrm dt = \int_{t_1}^{t_2} \left( \sum_{i=1}^N m_i\,\ddot{\bm r}_i \, \delta \bm r_i - \bm K_i \, \delta r_i \right) \, \mathrm dt = 0$$

                  

                  $$\implies \int_{t_1}^{t_2}
\left( 
\sum_{i=1}^N \left[ 
\frac{\mathrm d}{\mathrm dt} (m_i\,\dot{\bm r}_i\cdot \delta \bm r_i - \frac{m_i}{2}\delta\,\left(\dot{\bm r}_i^2\right) 
- \bm K_i\cdot \delta\bm r_i
\right] 
\right) \, \mathrm dt = 0$$

                  
                - Wegen [= 0 .](Analytische%20Mechanik/Grundkurs%20Theoretische%20Physik%202%20-%20Analytische%20Mechanik/Highlights/Page%20082/%3D%200%20.md) bleibt: 

                  $$\int_{t_1}^{t_2}
\left( 
\sum_{i=1}^N \left[ 
\frac{m_i}{2}\delta\,\left(\dot{\bm r}_i^2\right) 
+ \bm K_i\cdot \delta\bm r_i
\right] 
\right) \, \mathrm dt = 0$$

                  
                    - --------------------- Portal ---------------------
                        - Studium
                    - --------------------- Portal ---------------------
                        - Studium
                    - --------------------- Portal ---------------------
                        - Studium
                - Nach $(1.26)$ und $(1.29)$ ist

                  $$\sum_{i=1}^N \bm K_i \cdot \delta \bm r_i = \sum_{j=1}^S Q_j\cdot \delta q_j = - \sum_{j=1}^S \frac{\partial V}{\partial q_j} \, \delta q_j = -\delta V$$

                  
                - Somit wird $(1.124)$ zu 

                  $$\int_{t_1}^{t_2} \delta(T-V) \, \mathrm dt = \delta \int_{t_1}^{t_2}(T-V)\, \mathrm dt = \delta \int_{t_1}^{t_2} L \, \mathrm dt = 0$$

                  
            - 
        - ### Variationsrechnung
            - Wie können wir vom  *Wirkungsfunktional * auf die "stationäre" Bahn schließen?
                - --------------------- Portal ---------------------
                    - Studium
            - Aufgabe die Kurve zu finden, für die ein bestimmtes Linienintegral extremal wird ⇒ typisches  *Variationsproblem *  
            - ###### Konkurrenzschar,

              $$M \equiv \{ y(x)\,; \text{mindestens zweimal differenzierbar mit } \\
y(x_1) =y_1 \text{ und } y(x_2) =y_2$$

              
            - Allgemeines Funktional:

              $$J\{y(x)\} = \int_{x_1}^{x_2} f(x,y,y^\prime) \, \mathrm dx = \int_{x_1}^{x_2} \widetilde {f \,} (x) \ \mathrm dx$$

              
                - 

                  $$y^\prime =dy/dx, \; f(u,v,w) \text{ beliebig, stetig partiell diff.bar}$$

                  
            - Scharparameter $\alpha$
                - Hilfsmittel für das finden des $y(x)$, sodass die Bahn stationär ⇔ $J\{y(x)\}$ extremal wird
                - Stationär, wenn $y_{\alpha = 0}(x) = y_0(x)$ ⇒ gesucht
                - Parameterdarstellung: $y_\alpha(x) = y_0(x) +\gamma_\alpha(x)$ 
                    - Für $\gamma_\alpha$ soll gelten:
[„fast beliebige“](Analytische%20Mechanik/Grundkurs%20Theoretische%20Physik%202%20-%20Analytische%20Mechanik/Highlights/Page%20084/%E2%80%9Efast%20beliebige%E2%80%9C.md) Funktion,


                      $$\gamma_\alpha(x_1) = \gamma_\alpha(x_2) \equiv 0 \qquad \forall \,\alpha, \\ 
\ \\
\gamma_{\alpha=0}(x) \equiv 0 \qquad \forall \,x$$

                      
            - Wähle $\gamma_\alpha (x) = \alpha\, \eta(x), \quad \eta(x_1) = \eta(x_2) = 0$
                - Gute Wahl, weil $\alpha$ jetzt ein linearer Parameter is
                - [Taylorentwicklung](../../Taylorentwicklung.md)

                  $$\gamma_\alpha(x) = \alpha\,\left( \frac{\partial \gamma_\alpha(x)}{\partial \alpha}\right)_{\alpha\,=\,0} + \frac{\alpha^2}{2!} \left( \frac{\partial^2 \gamma_\alpha(x)}{\partial \alpha^2}\right)_{\alpha\,=\,0} + \mathcal{O}(\alpha^3)$$

                  
                - Einsetzen in ([1.127](Analytische%20Mechanik/Lagrange%20Mechanik/Hamilton%20Prinzip/Variationsrechnung/Scharparameter%20_alpha/Parameterdarstellung_%20y__alpha(x)%20%3D%20y_0(x)%20%2B_gamma__alpha(x).md))

                  $$y_\alpha = y_0(x)+\alpha\, \left( \frac{\partial \gamma_\alpha(x)}{\partial \alpha} \right)_{\alpha\,=\,0} + \dots$$

                  
                - Virtuelle Verschiebung bei festem $x$

                  $$\delta y = y_{\mathrm d\alpha}(x) - y_0(x) = \mathrm d\alpha\, \left(\frac{\partial \gamma_\alpha(x)}{\partial \alpha}\right)_{\alpha\,=\,0}$$

                  
            - ###### Variation des Funktionals $J\{y(x)\}$

              $$\delta J = J\{y_{\mathrm d\alpha}(x)\}-J\{y_0(x)\} = \left( \frac{\mathrm dJ(\alpha)}{\mathrm d\alpha} \right)_{\alpha\,=\,0} \mathrm d\alpha$$

              

              $$= \int_{x_1}^{x_2} \mathrm dx \,\big(f(x,y_{\mathrm d\alpha},y_{\mathrm d\alpha}')-f(x,y_0,y_0')\big).$$

              
            - ###### Euler'sche Gleichung

              $$\frac{\partial f }{\partial y} - \frac{\mathrm d}{\mathrm dx}\,\frac{\partial f}{\partial y'} = 0$$

              
                - ##### Herleitung:[Wähle y0(x) so, dass](Analytische%20Mechanik/Grundkurs%20Theoretische%20Physik%202%20-%20Analytische%20Mechanik/Highlights/Page%20085/W%C3%A4hle%20y0(x)%20so%2C%20dass.md)
                    - Wähle $y_0$ so, dass

                      $$\left( \frac{\mathrm dJ(\alpha)}{\mathrm d\alpha} \right)_{\alpha\,=\,0 } = 0 \quad \text{für } \textbf{beliebige } \gamma_\alpha(x)$$

                      
                    - $\alpha$ kann in den Integranden hereingezogen werden, $x$ wird nicht mitvariiert

                      $$\frac{\mathrm d}{\mathrm d \alpha} J(\alpha) = \int_{x_1}^{x_2} \mathrm d x \left( \frac {\partial f}{\partial y}\,\frac{\partial y}{\partial \alpha}+ \frac{\partial f}{\partial y'}\,\frac{\partial y'}{\partial \alpha} \right)$$

                      
                    - Erster Summand wird wegen ([1.128](Analytische%20Mechanik/Lagrange%20Mechanik/Hamilton%20Prinzip/Variationsrechnung/Scharparameter%20_alpha/Parameterdarstellung_%20y__alpha(x)%20%3D%20y_0(x)%20%2B_gamma__alpha(x)/F%C3%BCr%20_gamma__alpha%20soll%20gelten_%0A%E2%80%9Efast%20beliebige%E2%80%9C%20Funktion%2C%0A_gamma__alpha(x_1)%20%3D%20_gamma__alpha(x_2)%20_equiv%200%20_qquad%20_forall%20_%2C_alpha%2C%20__%20%0A_%20__%0A_gamma_%7B_alpha%3D0%7D(x)%20_equiv%200%20_qquad%20_forall%20_%2Cx.md)) zu 0 

                      $${\mathrm d \over \mathrm dx} J(\alpha) =\int_{x_1}^{x_2} \mathrm dx \left( \frac{\partial f}{\partial y}- \frac{\mathrm d}{\mathrm dx}\, \frac{\partial f}{\partial y'} \right) \frac{\partial y}{\partial \alpha}$$

                      
                    - Wegen ([1.129](Analytische%20Mechanik/Lagrange%20Mechanik/Hamilton%20Prinzip/Variationsrechnung/W%C3%A4hle%20_gamma__alpha%20(x)%20%3D%20_alpha_%2C%20_eta(x)%2C%20_quad%20_eta(x_1)%20%3D%20_eta(x_2)%20%3D%200/Virtuelle%20Verschiebung%20bei%20festem%20x_delta%20y%20%3D%20y_%7B_mathrm%20d_alpha%7D(x)%20-%20y_0(x)%20%3D%20_mathrm%20d_alpha_%2C%20_left(_frac%7B_partial%20_gamma__alpha(x)%7D%7B_partial%20_alpha%7D_right)_%7B_alpha_%2C%3D_%2C0%7D.md)) und ([1.130](Analytische%20Mechanik/Lagrange%20Mechanik/Hamilton%20Prinzip/Variationsrechnung/Variation%20des%20Funktionals%20J_%7By(x)_%7D_delta%20J%20%3D%20J_%7By_%7B_mathrm%20d_alpha%7D(x)_%7D-J_%7By_0(x)_%7D%20%3D%20_left(%20_frac%7B_mathrm%20dJ(_alpha)%7D%7B_mathrm%20d_alpha%7D%20_right)_%7B_alpha_%2C%3D_%2C0%7D%20_mathrm%20d_alpha%3D%20_int_%7Bx_1%7D%5E%7Bx_2%7D%20_mathrm%20dx%20_%2C_big(f(x%2Cy_%7B_mathrm%20d_alpha%7D%2Cy_%7B_mathrm%20d_alpha%7D')-f(x%2Cy_0%2Cy_0')_big).md)) auch

                      $$\delta J = \int_{x_1}^{x_2} \mathrm dx\,\left( \frac{\partial f }{\partial y} - \frac{\mathrm d}{\mathrm dx}\,\frac{\partial f}{\partial y'}\right)\ \delta y$$

                      
                    - Die Variation $\delta y$ ist [bis auf das Verschwinden an den Integralgrenzen beliebig.](Analytische%20Mechanik/Grundkurs%20Theoretische%20Physik%202%20-%20Analytische%20Mechanik/Highlights/Page%20086/bis%20auf%20das%20Verschwinden%20an%20den%20Integralgrenzen%20beliebig.md)
            - 
            - 
            - Anwendung: [Wir üben den Formalismus mit drei typischen Anwendungsbeispielen:](Analytische%20Mechanik/Grundkurs%20Theoretische%20Physik%202%20-%20Analytische%20Mechanik/Highlights/Page%20086/Wir%20%C3%BCben%20den%20Formalismus%20mit%20drei%20typischen%20Anwendungsbeispielen_.md)
            - [Wir haben zunächst die Variationstheorie des letzten Abschnitts auf mehrere Variablen zu verallgemeinern.](Analytische%20Mechanik/Grundkurs%20Theoretische%20Physik%202%20-%20Analytische%20Mechanik/Highlights/Page%20090/Wir%20haben%20zun%C3%A4chst%20die%20Variationstheorie%20des%20letzten%20Abschnitts%20auf%20mehrere%20Variablen%20zu%20verallgemeinern.md)
                - Analoge Herleitung für $S$ Koordinaten für **konservative Systeme** mit [Holonome Zwangsbedingungen](Analytische%20Mechanik/Lagrange%20Mechanik/Zwangsbedingungen/Holonome%20Zwangsbedingungen.md) 
                - Erweiterung für **konservative Systeme **mit **nicht-holonomen Zwangsbedingungen **für [Differentielle, nicht integrierbare Formen](Analytische%20Mechanik/Lagrange%20Mechanik/Zwangsbedingungen/Nicht-holonome%20Zwangsbedingungen/Differentielle%2C%20nicht%20integrierbare%20Formen.md)
            - 
        - ### Erhaltungssätze
            - --------------------- Portal ---------------------
                - Studium
            - Beispiel [Zweikörperproblem](Analytische%20Mechanik/Grundkurs%20Theoretische%20Physik%202%20-%20Analytische%20Mechanik/Highlights/Page%20099/Zweik%C3%B6rperproblem.md)
                - Es sind immer die [Generalisierte Koordinaten](Analytische%20Mechanik/Lagrange%20Mechanik/Generalisierte%20Koordinaten.md) zyklisch, die nur als Geschwindigkeit $(\dot q_j)$ vorkommen
                - Jede zyklische Koordinate liefert ein **Integral der Bewegung**
                - [Noether’sche Theoreme](Analytische%20Mechanik/Grundkurs%20Theoretische%20Physik%202%20-%20Analytische%20Mechanik/Highlights/Page%20101/Noether%E2%80%99sche%20Theoreme.md)
            - ### Homogenität der Zeit
                - ###### 

                  $$\textit{zeitliche Homogenität} \quad \iff \quad \frac{\partial L}{\partial t} = 0$$

                  
                - 

                  $$\frac{d}{dt}L
= \sum_{j=1}^{S}
\left(
\frac{\partial L}{\partial q_j}\,\dot q_j
+
\frac{\partial L}{\partial \dot q_j}\,\ddot q_j
\right) \
= \sum_{j=1}^{S}
\left[
\left(
\frac{d}{dt}
\frac{\partial L}{\partial \dot q_j}
\right)
\dot q_j
+
\frac{\partial L}{\partial \dot q_j}\,\ddot q_j
\right]
= \frac{d}{dt}
\sum_{j=1}^{S}
\frac{\partial L}{\partial \dot q_j}\,\dot q_j$$

                  
                    - Ausgenutzt wurde
                        - --------------------- Portal ---------------------
                            - Studium
                        - Umstellen 

                          $$\frac{d}{dt} \frac{\partial L}{\partial \dot q_j} = \frac{\partial L}{\partial q_j}$$

                          
                        - und

                          $$\ddot q_j = \frac{\mathrm d}{\mathrm dt}\,\dot q_j$$

                          
                - --------------------- Portal ---------------------
                    - Studium
                - ###### Hamilton-Funktion

                  $$H = \sum_{j=1}^Sp_j\dot q_j - L$$

                  
                - 

                  $$\text{Homogenität der Zeit} \:\Leftrightarrow \: \frac{\partial L}{\partial t} = 0, \\ \ \\

\text{"Systembewegung so, dass"} \: H = const.$$

                  
            - ### [Homogenität des Raumes](Analytische%20Mechanik/Grundkurs%20Theoretische%20Physik%202%20-%20Analytische%20Mechanik/Highlights/Page%20105/Homogenit%C3%A4t%20des%20Raumes.md) 
                - ###### 

                  $$\text{Homogenität des Raumes}\: \Leftrightarrow \: \text{Impulserhaltungssatz} \\ \ \\

\bm p = \sum_{i=1}^N m_i\, \dot{\bm r}_i = const.$$

                  
            - ### [Isotropie des Raumes](Analytische%20Mechanik/Grundkurs%20Theoretische%20Physik%202%20-%20Analytische%20Mechanik/Highlights/Page%20108/Isotropie%20des%20Raumes.md) 
                - ###### 

                  $$\text{Isotropie des Raumes } \Leftrightarrow \text{ Drehimpulserhaltungssatz}\\ \ \\
\bm L = \sum_{i=1}^N m_i\, \bm r_i \times \dot{\bm r}_i = const.$$

                  
            - 
        - 
    - 
- # Hamilton Mechanik
    - 

      $$\begin{array}{ccc}
& f(x) & \\
& \downarrow & \\
x = x(u) \longleftarrow &u = \dfrac{df}{dx} & \\
\searrow & \downarrow & \\
& f(x) - x \dfrac{df}{dx} &
\end{array}$$

      
    -  
    - 
- # Hamilton-Jacobi Theorie
- ## Übungsaufgaben Nolting
    - ### [Aufgabe 1.2.1](Analytische%20Mechanik/Grundkurs%20Theoretische%20Physik%202%20-%20Analytische%20Mechanik/Highlights/Page%20061/Aufgabe%201.2.1.md)
        - ### [Lösung zu Aufgabe 1.2.1](Analytische%20Mechanik/Grundkurs%20Theoretische%20Physik%202%20-%20Analytische%20Mechanik/Highlights/Page%20244/L%C3%B6sung%20zu%20Aufgabe%201.2.1.md)
            - [Gleitende Perle auf gleichförmig rotierendem Draht](Analytische%20Mechanik/Grundkurs%20Theoretische%20Physik%202%20-%20Analytische%20Mechanik/Highlights/Page%20037/2)%20Gleitende%20Perle%20auf%20gleichf%C3%B6rmig%20rotierendem%20Draht.md) 
            - Hier ist 

              $$T = \frac m2 (\dot x^2 + \dot y^2), \qquad V = 0 \quad(\text{Kein Potentialfeld})$$

              
            - und

              $$x = r\cos\omega t, \quad y = r\sin \omega t, \quad z = 0$$

              
            - Anders als typisch ist $r \neq const.$
            - Substituiere $r = q$
            - 

              $$\dot x = \dot q \cos\omega t - q\omega\sin\omega t \\
\ \\
\iff\dot x ^2 = \dot q^2 \cos^2\omega t - 2\dot q\cos{\omega t} \cdot q\omega\sin{\omega t} + q^2\omega^2\sin^2\omega t$$

              
            - 

              $$\dot y = \dot q\sin\omega t + q\omega\cos\omega t \\
\ \\
\iff \dot y^2 = \dot q^2\sin^2\omega t + 2\dot q \sin\omega t\cdot q\omega\cos\omega t + q^2\omega^2\cos^2\omega t$$

              
            - 

              $$\implies \dot x^2+ \dot y^2 = \dot q^2 + q^2\omega ^2$$

              
            - Lagrange DGL ⇒ [Lagrange-Gleichung (2. Art) \frac{d}{dt} \frac{\partial L}{\partial \dot q_j} - \frac{\partial L}{\partial q_j}   = 0, \qquad j =1,2,\dots, S](Analytische%20Mechanik/Lagrange%20Mechanik/Lagrange%20Gleichung/Der%20Regelfall%20von%20mechanischen%20Systemen%20ist%20ein%20konservatives%20System%20mit%20holonomen%20Zwangsbedingungen_/Lagrange-Gleichung%20(2.%20Art)%20_frac%7Bd%7D%7Bdt%7D%20_frac%7B_partial%20L%7D%7B_partial%20_dot%20q_j%7D%20-%20_frac%7B_partial%20L%7D%7B_partial%20q_j%7D%20%20%20%3D%200%2C%20_qquad%20j%20%3D1%2C2%2C_dots%2C%20S.md)

              $$\cancel m\,\ddot q - \cancel m \, q\omega ^2 = 0$$

              
                - 
    - ### [Aufgabe 1.2.2](Analytische%20Mechanik/Grundkurs%20Theoretische%20Physik%202%20-%20Analytische%20Mechanik/Highlights/Page%20062/Aufgabe%201.2.2.md) 
        - ### [Lösung zu Aufgabe 1.2.2](Analytische%20Mechanik/Grundkurs%20Theoretische%20Physik%202%20-%20Analytische%20Mechanik/Highlights/Page%20244/L%C3%B6sung%20zu%20Aufgabe%201.2.2.md)
            - Noch einmal [2) Gleitende Perle auf gleichförmig rotierendem Draht](Analytische%20Mechanik/Grundkurs%20Theoretische%20Physik%202%20-%20Analytische%20Mechanik/Highlights/Page%20037/2)%20Gleitende%20Perle%20auf%20gleichf%C3%B6rmig%20rotierendem%20Draht.md)
            - Es gibt zwei Zwangsbedingungen
                - 

                  $$\begin{align*}

f_1(\bm r,t) = z = 0 \quad &\to \quad \text{Nicht in der } z \text{-Ebene}\\
f_2(\bm r,t) = \varphi - \omega t = 0 \quad&\to\quad \text{Mit konstanter Winkelgeschwindigkeit} \Leftrightarrow \varphi = \omega t

\end{align*}$$

                  
                - --------------------- Portal ---------------------
                    - Studium
            - Mit Zylinderkoordinaten sehr einfach, es muss $\nabla_if_v$ gefunden werden:
                - --------------------- Portal ---------------------
                    - Studium
                - 

                  $$\implies \nabla f_1 = (0,0,1)=\bm e_z\,;\quad \nabla f_2 = \left(0, \frac1r, 0\right) = \frac1r\bm e_\varphi$$

                  
            - Damit liegt $\bm Z$ bis auf $\lambda$ fest

              $$\bm Z = \lambda_1 \bm e_z + \lambda_2\,\frac1r\,\bm e_\varphi$$

              
            - [Beschleunigung in Zylinderkoordinaten](../Physik/Klassische%20Mechanik/Grundkurs%20Theoretische%20Physik%201%20-%20Klassische%20Mechanik/Highlights/Page%20196/Beschleunigung%20in%20Zylinderkoordinaten.md):

              $$m\ddot{\bm r} = m \,(\ddot r-r\dot \varphi^2)\,\bm e_r+m\,(r\ddot\varphi+2\dot r\dot\varphi)\,\bm e_\varphi + m\ddot z \bm e_z \stackrel{!}{=} \bm Z + \underbrace{\bm K}_{=\,0}$$

              
                - Nach Zwangsbedingungen 

                  $$\ddot z = 0\,;\quad \dot \varphi = \omega\,;\quad \ddot \varphi=0\,.$$

                  
                - Zu lösen (komponentenweise, vergleiche Komponenten von $\bm Z$)

                  $$\left. \displaystyle \def\arraystretch{1.2} \begin{matrix}

m\,(\ddot r - \omega^2) &= 0 \\
2m\dot r \omega &= \lambda_2\,\frac1r \\
0 &= \lambda_1 

\end{matrix} 

\right\}

\implies \bm Z = 2m\dot r\omega \, \bm e_\varphi$$

                  
            - Erkennbar: $\bm Z \perp \bm e_r$
    - #### [Aufgabe 1.2.7](Analytische%20Mechanik/Grundkurs%20Theoretische%20Physik%202%20-%20Analytische%20Mechanik/Highlights/Page%20064/Aufgabe%201.2.7.md)
        - #### [Lösung zu Aufgabe 1.2.7](Analytische%20Mechanik/Grundkurs%20Theoretische%20Physik%202%20-%20Analytische%20Mechanik/Highlights/Page%20253/L%C3%B6sung%20zu%20Aufgabe%201.2.7.md)
            - ![](https://remnote-user-data.s3.amazonaws.com/EJx2Zte88GGg8gsVzU85iT2DK0haVqgOFZNQN6IBzLDyIGN3aOzS4wVlEJUrseMEpxR4ig19TPbmYIIsmOAYRo9rEmDZxUNW5hbVYzEEQk1BVJl2oegcONVvR-YWw5fu.png)
            - 

              $$r = \sqrt{x^2+y^2} \implies \tan\alpha = \frac{Ge}{An} = \frac rz$$

              
            - 

              $$\begin{align*}

x &=  r\cos\varphi \\
y &= r\sin\varphi \\
z &= r\cot\alpha

\end{align*}$$

              
            - --------------------- Portal ---------------------
                - Studium
        - 
    - #### [Aufgabe 1.2.13](Analytische%20Mechanik/Grundkurs%20Theoretische%20Physik%202%20-%20Analytische%20Mechanik/Highlights/Page%20068/Aufgabe%201.2.13.md) 
        - #### [Lösung zu Aufgabe 1.2.13](Analytische%20Mechanik/Grundkurs%20Theoretische%20Physik%202%20-%20Analytische%20Mechanik/Highlights/Page%20262/L%C3%B6sung%20zu%20Aufgabe%201.2.13.md)
            - $|\bm r| = l = const.$
                - Daraus folgt nicht notwendig, dass $\dot {\bm r} = 0$ 
                - --------------------- Portal ---------------------
                    - Studium
            - Schreibe $x^2+y^2+z^2 - l^2 = 0$ und $z = 0$
                - $S = 3-2 = 1$ Freiheitsgrad
                - Offensichtlich holonom, die Aufgabe bittet aber um Zwangskräfte
            - Wie komme ich auf den Term 

              $$\sum_{i=1}^{p} \lambda_i a_{im}\,?$$

              
                - Easy, tu so als wäre $x^2+y^2-l^2 = 0$ nicht holonom
                - Dazu

                  $$f(r,\varphi) = r^2\cos^2\varphi + r^2\sin^2\varphi - l^2 = 0 \iff r-l = 0$$

                  
                - Nun

                  $$\mathrm df = \mathrm dr  \implies a_r = 1,\,a_\varphi = 0$$

                  
                - Wir sehen ⇒ es gibt eine Zwangskraft in $r$-Richtung
                - Dann kannst du schreiben

                  $$\frac{\mathrm d}{\mathrm dt}\frac{\partial L}{\partial \dot r} - \frac{\partial L}{\partial r} = \lambda =\overline Q \longrightarrow \text{Fadenspannung}$$

                  
                - und

                  $$\frac{\mathrm d}{\mathrm dt}\frac{\partial L}{\partial \dot \varphi} - \frac{\partial L}{\partial \varphi} = 0 \longrightarrow \text{Bewegungsgleichung}$$

                  
    - #### [Aufgabe 1.3.3](Analytische%20Mechanik/Grundkurs%20Theoretische%20Physik%202%20-%20Analytische%20Mechanik/Highlights/Page%20096/Aufgabe%201.3.3.md)
        - #### [Lösung zu Aufgabe 1.3.3](Analytische%20Mechanik/Grundkurs%20Theoretische%20Physik%202%20-%20Analytische%20Mechanik/Highlights/Page%20305/L%C3%B6sung%20zu%20Aufgabe%201.3.3.md)
            - ![](https://remnote-user-data.s3.amazonaws.com/_FQUcLiR0NEATdimoHS-_fFXQvOEJFWthilE_Nf63nMWYYt45aMJx_Eyau3SWdd5ptxl_k4GvlLPr7Tj4mCU8ZJG3dugi5GDd8bqGmHPNkEYQ6zun3YfOrF4Bl1hR5k6.png)
                - Kinetische Energie→

                  $$T = \frac12\int_0^lm(x) \,\dot y^2 \,\mathrm dx\,\quad m(x) =\frac{\mathrm dm}{\mathrm dx}$$

                  
                - Potentielle Energie $V$
                    - Ansatz→

                      $$V=\alpha\left(\int_0^l\mathrm ds - l\right)\,; \quad \mathrm ds = \sqrt{\mathrm dx^2 +\mathrm dy^2}$$

                      
                - Kinetische Energie $T$→

                  $$T =\frac12 \int\limits_0^l m(x)\,\dot y^2\,\mathrm dx\,,\quad m(x) = \frac{\mathrm dm}{\mathrm dx}$$

                  
                - Potentielle Energie $V$→

                  $$V = \alpha \left( \,\int\limits_0^l ds - l\,\right), \quad ds = \sqrt{x^2+y^2}$$

                  
                    - Mit $y' = \mathrm dy/\mathrm dx$

                      $$V=\alpha\left( \int\limits_0^l {{c1::\sqrt{1+y'^2}\,\mathrm dx }}- l\right)$$

                      
            - Für kleine Auslenkungen gilt 

              $$\sqrt{1+y'^2} \approx {{c1::1+\frac12y'^2}}$$

              
                - 

                  $$V \approx \frac\alpha2\,\int\limits_0^ly'^2\,\mathrm dx \iff \int\limits_0^l1\,\mathrm dx -l = 0$$

                  
                - 
            - Forderung $\delta S = 0$, damit

              $$0 \overset{!}{=} \delta S
= \int_{t_1}^{t_2} \int_{0}^{l}
\left(
m(x)\,\dot{y}\,\delta \dot{y}
- a\,y'\,\delta y'
\right)
\, dx\, dt$$

              
                - --------------------- Portal ---------------------
                    - Studium
            - 

              $$\delta S= \int_{0}^{l} m(x)\,\big[\,\dot y\,\delta y\,\big]_{t_1}^{t_2}\,dx
\;-\;
\alpha \int_{t_1}^{t_2} \big[\,y'\,\delta y\,\big]_{0}^{l}\,dt
\;-\;
\int_{t_1}^{t_2}\int_{0}^{l}
\big(m(x)\,\ddot y - \alpha\,y''\big)\,\delta y
\,dx\,dt .$$

              
                - Nun: Hardcore [Partielle Integration](../../Studium/Mathe%20Basics/Partielle%20Integration.md)

                  $$-\alpha\!\int\limits_{t_1}^{t_2} \int\limits_0^l\,y'\delta y' \, \mathrm dx\mathrm dt = - \alpha\! \int\limits_{t_1}^{t_2} \big[y'\delta y\big]_0^l\,\mathrm dt + \alpha \!\int\limits_{t_1}^{t_2}\int\limits_0^l y''\,\delta y\,\mathrm dx\,\mathrm dt

\\ \ \\

\int\limits_0^l \int\limits_{t_1}^{t_2} m(x)\,\dot y\,\delta \dot y \,\mathrm dx \,\mathrm dt = \int\limits_0^lm(x)\,\big[\dot y\,\delta  y\big]_{t_1}^{t_2}\,\mathrm dx - \int\limits_0^l \int\limits_{t_1}^{t_2} m(x)\,\ddot y\,\delta y \,\mathrm dx \,\mathrm dt$$

                  
            - Verschwindet an den Grenzen also 

              $$0 = -\;
\int_{t_1}^{t_2}\int_{0}^{l}
\big(m(x)\,\ddot y - \alpha\,y''\big)\,\delta y
\,dx\,dt .$$

              
            - $\delta y$ ist beliebig!

              $$m(x)\,\ddot y - \alpha\,y'' = 0 \iff m(x)\frac{\partial^2y}{\partial t^2} = \alpha \frac{\partial^2 y}{\partial x^2}$$

              
    - 1.3.5
    - 1.4.2
    - 
- Grundkurs Theoretische Physik 2 - Analytische Mechanik 
    - 
    - 
