#### №1
Найти среднее по времени значение тензора $E_\alpha(t) B_\beta(t - \tau)$  для электромагнитной  волны с левой круговой поляризацией в вакууме. Амплитуда волны $E$, волновой вектор $\vec \kappa$, и фаза запаздывания  $\varphi = \kappa c \tau$, заданы. Как изменится ответ для линейно поляризованной волны
***
**Решение**:
	Используем Фурье — представление:
$rot E = - \frac {1}{c}\frac{\partial B}{\partial t} \Rightarrow i[\kappa \times E] = \frac {i \omega B}{c} \Rightarrow B_\beta = [\vec \kappa \times \vec E]_\beta = \frac{e_{\beta n s} \kappa_n E_s c}{\omega}$
$<E_\alpha(t)B_\beta(t-\tau)> = <e_{\beta n s} \frac{c}{\omega} \kappa_n E_s(t-\tau)E_\alpha(t)> = \frac{c}{\omega}e_{\beta n s}\kappa_n<E_\alpha(t)E_s(t-\tau)$
, где $\kappa_n$ не зависит от времени.
Т.к. поляризация круговая, то тензор инвариантен относительно поворота вокруг $z(z||\kappa)$
Имеем тензор второго ранга:
$<E_\alpha(t)E_s(t-\tau)> = A\delta_{\alpha s} + B\kappa_\alpha \kappa_s + C e_{\alpha s \gamma}\kappa_\gamma$
Данный тензор имеет 5 ненулевых компонентов. Для левой части это — фаза, амплитуда, поляризация, направление
Найдем $A, B, C$. Домножим на $\delta_{\alpha s}$. Учтем, что $\delta_{\alpha\alpha} = 3, e_{\alpha\alpha\gamma} = 0, \kappa_\alpha \kappa_\alpha = \kappa^2; E_\alpha(t)E_s(t-\tau)\delta_{\alpha s} = E^2\cos\varphi$, т.е. $\alpha = s$
$E^2\cos\varphi = 3A + B\kappa^2$
Сделаем свертку с $\kappa_\alpha \kappa_\alpha$, т.к. $\vec E \vec \kappa = 0$ (все электромагнитные волны в вакууме)
Слева: $<E_\alpha(t)E_s(t-\tau)>\kappa_\alpha \kappa_\alpha =  <E_\alpha(t)E_s(t-\tau)\kappa_\alpha \kappa_\alpha>$ = 0
Справа: $0 = A\kappa^2 + B\kappa^4$.
Свертка с $e_{\alpha s n}$, учтем, что $e_{\alpha s \gamma} e_{\alpha s q} = 2 \delta_{\gamma q}$
$E_\alpha E_s(t-\tau)e_{\alpha s q} = -E^2\sin\varphi \frac{\vec \kappa}{\kappa} = 2\delta_{\alpha q}C\kappa_\gamma \Rightarrow C = \frac{-E^2\sin\varphi}{2\kappa}$
$E^2\cos\varphi - 3A = B\kappa^2$
$\begin{cases} A + B\kappa^2 = 0 \\ A = \frac{E^2\cos\varphi}{2} \end{cases}$
$B = \frac{E^2\cos\varphi}{\kappa^2}-\frac{3E^2\cos\varphi}{\kappa^2} \Rightarrow B = -\frac{E^2\cos\varphi}{2\kappa^2}$
Итого:
$\begin{cases} A = \frac{E^2\cos\varphi}{2}, \\ B = -\frac{E^2\cos\varphi}{2\kappa^2},\\ C = \frac{-E^2\sin\varphi}{2\kappa}. \end{cases}$
Подставим полученные коэффициенты: $<E_\alpha(t)E_s(t-\tau)> = \frac{E^2\cos\varphi}{2}\delta_{\alpha s}  -\frac{E^2\cos\varphi}{2\kappa^2}\kappa_\alpha \kappa_s + \frac{-E^2\sin\varphi}{2\kappa} e_{\alpha s \gamma}\kappa_\gamma$
Свернем $<E_\alpha E_s>$ с тензором $e_{\beta n s} \frac{c}{\omega} \kappa_n$
$<E_\alpha E_\beta> = [\delta_{\alpha s} e_{\beta n s} \kappa_n = e_{\beta n \alpha} \kappa_n; \kappa_\alpha \kappa_s e_{\beta n s} \kappa_n = \kappa_\alpha[\vec \kappa\times\vec\kappa] = 0;$
$ e_{\alpha s \gamma}\kappa_\gamma e_{\beta n s} \kappa_n = \kappa_n \kappa_\gamma(e_{\beta n s}e_{\alpha s \gamma})=(-\delta_{\beta\alpha}\delta_{n \gamma} +\delta_{\beta\alpha}\delta{\beta\alpha})\kappa_n\kappa_\gamma= -\kappa^2\delta_{\beta \alpha}+\kappa_n \kappa_\gamma]$
**Получим:** $<E_\alpha E_\beta> = \frac{cE^2\cos\varphi e_{\beta n \alpha} \kappa_n}{2\omega} +\frac{E^2c\sin\varphi\vec\kappa\delta_{\beta\alpha}}{2\omega}-\frac{E^2c\sin\varphi\kappa_n\kappa_\gamma}{2\kappa\omega}$
***
Для линейно поляризованной волны выберем направление $\vec n = \frac {\vec E}{E} $, т.к. $\vec\kappa$ не определяет направление поля однозначно.
$E_\alpha = E n_\alpha\cos\omega t$
$B_\beta = e_{\beta n s} \kappa_n E_s \frac{c}{\omega} = E e_{\beta n s}\kappa_n \kappa_s \cos(\omega t - \varphi)$
$<E_\alpha(t)B_\beta(t-\tau)> = \frac{c}{\omega}E^2n_\alpha n_s e_{\beta b s} \kappa_n <\cos{\omega t}\cos(\omega t -\varphi)>$
Рассматриваем только $<\cos{\omega t}\cos(\omega t -\varphi)>$
$\cos(\alpha - \beta) = \cos\alpha\cos\beta +\sin\alpha\sin\beta$
$<\cos{\omega t}\cos(\omega t -\varphi)> = <\cos^2{\omega t} \cos \varphi + \sin{\omega t}\sin\varphi\cos{\omega t}> = $
$=\begin{bmatrix}\cos^2{\omega t} = \frac{1}{2}\\
<\sin{\omega t}\cos t> = 0 \end{bmatrix} = \frac{1}{2}\cos\varphi$

**Ответ:**
$<E_\alpha(t)B_\beta(t-\tau)> =  \frac{1}{2}\frac{c}{\omega}\cos\varphi E^2n_\alpha n_s e_{\beta b s} \kappa_n $


***
#### №2
Найти диэлектрическую проницаемость однородного электролита с положительными (s = 1) и отрицательными (s = 2) ионами, если известно, что плотность потока частиц сорта s имеет вид  $f^s = n^s b^s q^s \vec E - D^s \nabla n^s$,   где $q^s$- заряд, $b^s$- подвижность, $D^s$ - коэффициент диффузии, $n^s$- концентрация ионов, причём отношение $\frac{D^s}{b^s}=kT$ зависит только от температуры. Найти поле неподвижного точечного заряда в такой среде.
***
**Решение:**
Ищем диэлектрическую проницаемость:
Имеем плотность потока: $f^s = n^s b^s q^s \vec E - D^s \nabla n^s$
Связь с плотностью тока: $j = \sum f^s q^s$
Для того, чтобы перейти в Фурье пространство, нужно  линеаризовать все компоненты.
1) $f = f_0 + \delta f$
2) $n = n_0 + \delta n$
3) $b = b_0 + \delta b$
4) $D = D_0 + \delta D$
5) $E = E_0 + \delta E$

Из условия $\frac{D^s}{b^s}=kT$ можно заменить, что $D$ и $b$ линеаризовать не нужно, но для профилактики проверим и их.
$f_0 + \delta f = (n_0 + \delta n)(b_0 + \delta b)q(E_0 + \delta E) - (D_0 + \delta D) \vec \nabla (n_0 + \delta n) = $
$= (n_0 b_0 + n_0 \delta b + \delta n b_0 + \delta n \delta b)q(E_0 + \delta E) = qn_0 b_0 E_0 + n_0 q E_0 \delta b + \delta n b_0 q E_0 +$
$+\delta n \delta b q E_0 + n_0 b_0 q \delta E + n_0 \delta b q \delta E + \delta n b_0 q \delta E + \delta n \delta b q \delta E - (D_0n_0 + D_0 \delta n + \delta D n_0 +$
	$+ \delta D \delta n)\vec \nabla = qn_0b_0E_0 + n_0qE_0\delta b + \delta n b_0 q E_0 +n_0 b_0q \delta E - \vec\nabla D_0 n_0 - D_0\vec\nabla\delta n- $
	$-\vec\nabla\delta D n_0 - \vec\nabla\delta D \delta n = q n_0b_0 E_0 + \delta n b_0 q E_0 + n_0 b_0 q \delta E - D_0\vec\nabla\delta n = f_0 + \delta f$
	Исключим малые компоненты. Оставим только линейные.
	$f_0 = qn_0b_0 E_0$, где $f_0$ - стационарный поток. В условии не говорится о его существовании $\Rightarrow f_0 = 0 \Rightarrow E_0 = 0$
	В итоге:
	$\delta f = n_0 b_0 q \delta E - D_0 \nabla \delta n$
	Теперь переходим в пространство Фурье.
	$j(\kappa, \omega) = f^s(\kappa, \omega)q^s = [\vec\nabla \rightarrow i \kappa]= n_0^sb_0^sq^{s^2}\vec E(\kappa, \omega) - i D^s \kappa \delta n^s q^s$ *(1)*
	Также для каждого малого объема должно выполняться уравнение непрерывности:
	$div\delta j + \frac{\partial \rho_0}{\partial t}=0$
	При переходе в пространство Фурье $[div \vec j \rightarrow i(\vec\kappa\delta \vec j)(\kappa, \omega), \frac{\partial}{\partial t} \rightarrow - i\omega]$
	$i(\vec\kappa, \delta \vec j)(\kappa, \omega) = i\omega\rho(\kappa, \omega) = i\omega q^sn^s(\kappa, \omega) \text{ (2)} \Rightarrow (\vec\kappa\delta\vec j^s) = \omega q^s \delta n^s$
	Нужно получить $j$ в виде $\delta j_\alpha = \sigma_{\alpha \beta} E_\beta$
	Домножим *(1)* скалярно на $\vec\kappa$
	$(\delta \vec j^s, \vec \kappa) = n_0^sb_0^sq^{s^2}(\vec E \vec \kappa) - i D^s \kappa^2\delta n^s q^s$
	Подставим *(2)* в последнее уравнение
	$(\delta\vec j^s, \vec\kappa) = n_0^s b_0^s q^{s^2}(\vec E \vec \kappa) - i D^s \frac{\kappa^2}{\omega}\delta(\delta\vec j^s, \vec\kappa)$
	Выразим $(\delta\vec j^s, \vec\kappa)$:
	$(\delta\vec j^s, \vec\kappa) = \frac{n_0^s b_0^s q^{s^2}(\vec E \vec \kappa)}{1+ i D^s \frac{\kappa^2}{\omega}}$
	С другой стороны:
	$j_\alpha^s = n_0^sb_0^sq^{s^2}\vec E(\kappa, \omega) - i D^s \frac{\vec\kappa}{\omega}(\delta\vec j \vec \kappa)$
	$j_\alpha^s = n_0^sb_0^sq^{s^2}\vec E(\kappa, \omega) - i D^s \frac{\vec\kappa}{\omega}\frac{n_0^s b_0^s q^{s^2}(\vec E \vec \kappa)}{1+ i D^s \frac{\kappa^2}{\omega}}$
	Перейдем к тензорному представлению
	$j_\alpha^s = n_0^sb_0^sq^{s^2} E_\beta - i D^s \frac{\kappa_\alpha}{\omega}\frac{n_0^s b_0^s q^{s^2}(E_\beta \kappa_\beta)}{1+ i D^s \frac{\kappa^2}{\omega}}$
	$\Downarrow$
	$j_\alpha^s = E_\beta(n_0^sb_0^sq^{s^2} \delta_{\alpha\beta}) -  i \frac{ D^s}{\omega}\frac{n_0^s b_0^s q^{s^2}\kappa_\alpha \kappa_\beta}{1+ i D^s \frac{\kappa^2}{\omega}}$
	т.е.
	$\sigma_{\alpha \beta} = \sum\limits_{s=1,2} n_0^sb_0^sq^{s^2} \delta_{\alpha\beta} -\frac{i D^s n_0^s b_0^s q^{s^2}\kappa_\alpha \kappa_\beta}{\omega+ i D^s \kappa^2}$
	$\sigma_{\alpha \beta} = \sum\limits_{s=1,2} n_0^sb_0^sq^{s^2} \delta_{\alpha\beta} -\frac{i D^s n_0^s b_0^s q^{s^2}\kappa_\alpha \kappa_\beta}{i(\frac{\omega}{i} + i D^s \kappa^2)}= \sum\limits_{s=1,2} n_0^sb_0^sq^{s^2} \delta_{\alpha\beta} -\frac{D^s n_0^s b_0^s q^{s^2}\kappa_\alpha \kappa_\beta}{ D^s \kappa^2 - i\omega}$
	Получаем диэлектрическую проницаемость
	$\varepsilon_{\alpha\beta} = \delta_{\alpha\beta} + \frac{4\pi i}{\omega}\sum\limits_{s=1,2} n_0^sb_0^sq^{s^2}(\delta_{\alpha\beta} -\frac{D^s \kappa_\alpha \kappa_\beta}{ D^s \kappa^2 - i\omega})$
***
Найдем поле:
$\begin{cases}div D = 4\pi \rho \\
-\nabla\varphi = \vec E\end{cases}$
Фурье представление
$i\vec\kappa\vec D = 4\pi \rho \Rightarrow i \kappa_\beta\varepsilon_{\alpha\beta}E_\beta = 4\pi\rho(\kappa, \omega)$;
$-\vec\kappa\varphi = \vec E \Rightarrow -i \kappa_\alpha\varphi = E_\alpha$.
$\rho(r, t) = \delta(r, t) q \Rightarrow$ Ф.п.
$\rho(\kappa, \omega) =\frac{1}{(2\pi)^2}\int\delta(r)e^{-i\kappa r + i \omega t}d\vec r dt = \frac{1}{(2\pi)^2}\int e^{i\omega t}dt = \frac{1}{(2\pi)^2}\delta(\omega)$
$\rho(\kappa, \omega) = \frac{1}{(2\pi)^2}\delta(\omega) q$
В итоге $\varepsilon_{\alpha\beta}\kappa_\alpha\kappa_\beta\varphi = 2q\delta(\omega)$
$\varphi(\kappa,\omega) = \frac{2q\delta(\omega)}{\kappa_\alpha\kappa_\beta\varepsilon_{\alpha\beta}}$
Произведем свертку
$\kappa_\alpha\kappa_\beta\varepsilon_{\alpha\beta} = \kappa_\alpha\kappa_\beta\delta_{\alpha\beta}+\frac{4\pi i}{\omega}\sum\limits_{s = 1,2}n_0^sb_0^sq^{s^2}(\kappa_\alpha\kappa_\beta\delta_{\alpha\beta} -\frac{D^s \kappa_\alpha \kappa_\beta\kappa_\alpha \kappa_\beta}{ D^s \kappa^2 - i\omega})=$
$=\kappa^2 + \frac{4\pi i}{\omega} \sum n_0^sb_0^sq^{s^2}(\kappa^2 -\frac{D^s \kappa^4}{ D^s \kappa^2 - i\omega}) = \kappa^2 + \frac{4\pi i}{\omega} \sum n_0^sb_0^sq^{s^2}(\frac{D^s \kappa^4-D^s\kappa^4-i\omega\kappa^2}{ D^s \kappa^2 - i\omega})=$
$=\kappa^2 + \frac{4\pi \kappa^2}{\omega} \sum \frac{n_0^sb_0^sq^{s^2}}{ D^s \kappa^2 - i\omega}$.
Вернемся к нормальным координатам
$\varphi(r, t) = \frac{1}{(2\pi)^2}\int\frac{2q\delta(\omega)e^{i(\kappa r - \omega t)}}{\kappa^2+\sum{\frac{4\pi\kappa^2 n^s b^s q^{s^2}}{D^s\kappa^2 -i\omega}}}d^3\kappa d\omega =$ интегрируем по $\omega=$
$=\frac{2q}{(2\pi)^2}\int\frac{e^{i\vec\kappa \vec r}}{\kappa^2+\sum{\frac{4\pi\kappa^2 n^s b^s q^{s^2}}{D^s}}}d^3\kappa $
 сделаем замену $\varkappa^2 = \frac{4\pi n^s b^s q^{s^2}}{D^s}$ - Дебаевский радиус
 $=\frac{2q}{(2\pi)^2}\int\frac{e^{i\vec\kappa\vec r}}{\kappa^2 + \varkappa^2}d^3\kappa = $
 Перейдем в сферическую систему координат
 $=\frac{2q}{(2\pi)^2}\int\limits_0^{2\pi}\int\limits_0^\pi\int\frac{e^{i\kappa r \cos\theta}}{\kappa^2+\varkappa^2}\kappa^2\sin\theta d\theta d\varphi$
$\begin{cases}
d^3\kappa = \kappa^2\sin\theta d\theta d\varphi \\
\kappa_x = \kappa\sin\theta\cos\varphi \\
\kappa_y = \kappa\sin\theta\sin\varphi \\
\kappa_z = \kappa\cos\theta
\end{cases}$
интегрируем по $\varphi$
$\frac{2q\cdot 2\pi}{(2\pi)^2}\int\limits_0^\infty[\int\limits_0^\pi e^{i\kappa r \cos\theta}\sin\theta d\theta]\frac{\kappa^2}{\kappa^2+\varkappa^2}d\kappa = $
интегрируем по $\theta$
$\frac{2q\cdot 2\pi}{(2\pi)^2}\int\limits_0^\infty \frac{-e^{i\kappa r \cos\theta}}{i\omega r} \Big|_0^\pi \frac{\kappa^2}{\kappa^2+\varkappa^2}d\kappa = \frac{q}{\pi}\int\limits_0^\infty\frac{-e^{i\kappa r}+e^{i\kappa r}}{i\kappa r}\frac{\kappa^2}{\kappa^2+\varkappa^2}d\kappa=\frac{2q}{\pi r}\int\limits_0^\infty\frac{\sin{\kappa r}\kappa}{\kappa^2+\varkappa^2}d\kappa =$
используем нечетность $sin$
$\frac{q}{\pi r}\int\limits_{-\infty}^\infty\frac{\sin{\kappa r}\kappa}{\kappa^2+\varkappa^2}d\kappa = \frac{q}{\pi r} Im \int\frac{e^{i\kappa r}}{\kappa^2 + \varkappa^2}\kappa d\kappa = \frac{q}{\pi r} Im 2\pi i(Res(\frac{e^{i\kappa r}\kappa}{\kappa^2+\varkappa^2}))$
Приведем вычет $2\pi i(Res(\frac{e^{i\kappa r}\kappa}{\kappa^2+\varkappa^2}))$ к кошерному виду
$\kappa^2 + \varkappa^2 = 0$
$\kappa = \pm i\varkappa$ - полюс первого порядка
Сделаем замену $\frac{\kappa^2}{\varkappa^2}=y^2$
$2\pi i(Res(\frac{e^{i\kappa r}\kappa}{1+y^2}))=2\pi i(Res(\frac{e^{i\kappa r}\kappa}{(y-i)(y+i)}))$
Чтобы понять как будет обходить точку, сверху или снизу, нужно проверить интеграл
$\int\limits_{-\infty}^\infty \frac{\kappa\sin{\kappa r}}{\kappa^2+\varkappa^2}d\kappa=Im\int\limits_{-\infty}^\infty \frac{\kappa e^{i\kappa r}}{\kappa^2+\varkappa^2}d\kappa=[\text{замена }\kappa = R\cdot e^{i\varphi}]=$
$=\int\limits_0^\pi\frac{R e^{i\varphi} e^{iRe^{i\varphi}r}Rie^{i\varphi}d\varphi}{R^2e^{2i\varphi}-\varkappa^2}=\int\limits_0^\pi\frac{e^{iRe^{i\varphi}r}ie^{i2\varphi}d\varphi}{e^{i2\varphi}+\frac{\varkappa^2}{R^2}}=[\text{при }R \to \infty \Rightarrow \frac{\varkappa^2}{R^2}\to 0]=$
$=\int i e^{iR(\cos{\varphi}+i\sin\varphi)r}d\varphi = \int i e^{iRr\cos{\varphi}} e^{-Rr\sin{\varphi}}d\varphi$
Видим, что $ ie^{iRr\cos{\varphi}}$ ограничен, а $e^{-Rr\sin{\varphi}}$ сходится только при $\sin{\varphi}<0$
Следовательно делаем обход сверху.
![](picture2.png)
*(Направление обхода обуславливается пределами интеграла $(-\infty ; \infty)$)*
Получаем
$\frac{q}{\pi r} Im 2\pi i \frac{e^{-i r \varkappa}\kappa}{2\kappa}=\frac{q}{r}e^{-2\varkappa}$
В итоге потенциал равен:
$\varphi = \frac{q}{r}e^{-2\varkappa}$
Найдем поле:
$E=-\nabla \varphi=-\frac{\vec r}{r}\frac{\partial\varphi}{\partial r}=-\frac{\vec r}{r}q(-\frac{-\varkappa e^{-r\varkappa}}{r}-\frac{e^{-r\varkappa}}{r^2})=\frac{q\vec r}{r}(\varkappa r e^{-r\varkappa}+e^{-r\varkappa})=\frac{q\vec r}{r^3}e^{-r\varkappa}(r\varkappa+1)$
***
##### №3
Плоская монохроматическая электромагнитная волна с круговой поляризацией падает из вакуума по нормали на плоскую поверхность одноосного кристалла с диэлектрической проницаемостью $\varepsilon_{\alpha\beta} =2.25 \delta_{\alpha\beta} +9.75 h_\alpha h_\beta$. Под каким углом к нормали направлена ось кристалла $h$, если известно, что отражённая волна имеет эллиптическую поляризацию с отношением осей 17:35?
***
**Решение:**
$L_{\alpha\beta}E_\beta = (\kappa_\alpha\kappa_\beta - \kappa^2\delta_{\alpha\beta}+\frac{\omega^2}{c^2}\varepsilon_{\alpha\beta})E_\beta = 0$
$\vec E = (E_x0, E_y0, 0);$
$\vec n =(\sin\theta,0,\cos\theta);$
$\vec\kappa = (0,0,\kappa_z);$
$\begin{pmatrix}
-\kappa^2 +\frac{\omega^2}{c^2}((\varepsilon_\perp-\varepsilon_\perp\sin^2\theta)+\varepsilon_\parallel\sin^2\theta) & 0 & \frac{\omega^2}{c^2}(-\varepsilon_\perp\sin\theta\cos\theta+\varepsilon_\parallel\sin\theta\cos\theta)\\0 & -\kappa^2 +\frac{\omega^2}{c^2}\varepsilon_\perp & 0 \\ \frac{\omega^2}{c^2}(-\varepsilon_\perp\sin\theta\cos\theta+\varepsilon_\parallel\sin\theta\cos\theta) & 0 & \frac{\omega^2}{c^2}((\varepsilon_\perp-\varepsilon_\perp\cos^2\theta)+\varepsilon_\parallel\cos^2\theta)
\end{pmatrix}$
$det L_{\alpha\beta}= 0;$
Найдем обыкновенную и необыкновенную волны
$\begin{pmatrix} A & 0 & B\\ 0 & 0 & 0\\ C & 0 & D
\end{pmatrix} \begin{pmatrix}0\\E_y\\0\end{pmatrix} = \begin{pmatrix}0\\0\\0\end{pmatrix}$ - обыкновенная волна

$\begin{pmatrix} 0 & 0 & 0\\ 0 & A & 0\\ 0 & 0 & 0
\end{pmatrix} \begin{pmatrix} E_x\\0\\E_z\end{pmatrix} = \begin{pmatrix}0\\0\\0\end{pmatrix}$- необыкновенная волна
Для обыкновенной волны:
$\kappa^2= \frac{\omega^2}{c^2}\varepsilon_\perp, E_y \ne 0$
$(\kappa^2= \frac{\omega^2}{c^2}\varepsilon_\perp)E_y = 0$
$\omega = \kappa c \sqrt\frac{1}{\varepsilon_\perp}$
*Скорость распространения обыкновенной волны $v = \frac{c}{n}, n = \sqrt{\varepsilon\mu}$
У необыкновенной волны скорость распространения зависит от угла между направлением нормали и оптической осью.*
Для необыкновенной волны:
$(-\kappa^2 +\frac{\omega^2}{c^2}(\varepsilon_\perp-\varepsilon_\perp\sin^2\theta+\varepsilon_\parallel\sin^2\theta))\frac{\omega^2}{c^2}(\varepsilon_\perp-\varepsilon_\perp\cos^2\theta+\varepsilon_\parallel\cos^2\theta)-$
$-\frac{\omega^4}{c^4}(-\varepsilon_\perp\sin\theta\cos\theta+\varepsilon_\parallel\sin\theta\cos\theta) = 0$
$-\kappa^2 +\frac{\omega^2}{c^2}((\varepsilon_\perp-\varepsilon_\perp\sin^2\theta)+\varepsilon_\parallel\sin^2\theta) = \frac{\omega^2}{c^2}(\frac{(\varepsilon_\parallel - \varepsilon_\perp)^2\sin^2\theta\cos^2\theta}{\varepsilon_\perp + \cos^2\theta(-\varepsilon_\perp + \varepsilon_\parallel)})$
$\kappa^2 = \frac{\omega^2}{c^2}((\varepsilon_\perp(-\varepsilon_\perp+\varepsilon_\parallel)\sin^2\theta) - \frac{(\varepsilon_\parallel - \varepsilon_\perp)\sin^2\theta\cos^2\theta}{\varepsilon_\perp +\cos^2\theta(-\varepsilon_\perp + \varepsilon_\parallel)}) = $
$= \frac{\omega^2}{c^2}(\frac{\varepsilon_\perp(\varepsilon_\perp +\cos^2\theta(-\varepsilon_\perp+\varepsilon_\parallel)+(-\varepsilon_\perp+\varepsilon_\parallel)\sin^2\theta(\varepsilon_\perp+\cos^2\theta(-\varepsilon_\perp+\varepsilon_\parallel)}{\varepsilon_\perp +\cos^2\theta(-\varepsilon_\perp + \varepsilon_\parallel)} - \frac{(\varepsilon_\parallel-\varepsilon_\perp)^2\sin^2\theta\cos^2\theta}{\varepsilon_\perp + \cos^2(-\varepsilon_\perp+\varepsilon_\parallel)})=$
$=\frac{\omega^2}{c^2}(\frac{\varepsilon^2_\perp+\varepsilon_\perp\cos^2\theta(-\varepsilon_\perp+\varepsilon_\parallel)+\varepsilon_\perp(-\varepsilon_\perp+\varepsilon_\parallel)\sin^2\theta-(\varepsilon_\parallel-\varepsilon_\perp)^2\sin^2\cos^2\theta}{\varepsilon_\perp+\cos^2\theta(-\varepsilon_\perp+\varepsilon_\parallel)})$
$\kappa^2 = \frac{\omega^2}{c^2}(\frac{\varepsilon^2_\perp+\varepsilon_\perp\cos^2\theta(-\varepsilon_\perp + \varepsilon_\parallel)+\varepsilon_\perp(-\varepsilon_\perp+\varepsilon_\parallel)\sin^2\theta}{\varepsilon_\perp+\cos^2\theta(-\varepsilon_\perp+\varepsilon_\parallel)})$
$\kappa^2 = \frac{\omega^2}{c^2}(\frac{\varepsilon^2_\perp+\varepsilon_\perp(-\varepsilon_\perp+\varepsilon_\parallel)}{\varepsilon_\perp +\cos^2\theta(-\varepsilon_\perp+\varepsilon_\parallel)})$
Скорость распространения необыкновенной волны:
$v = \frac{c}{\sqrt{\frac{\varepsilon^2_\perp+\varepsilon_\perp(-\varepsilon_\perp+\varepsilon_\parallel)}{\varepsilon_\perp +\cos^2\theta(-\varepsilon_\perp+\varepsilon_\parallel)}}}$
