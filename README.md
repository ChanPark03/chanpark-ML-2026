# chanpark-ML-2026

Machine learning, deep learning studying repo.

이 README는 짧은 소개 문서가 아니라, NumPy, Matplotlib, Pandas 학습 내용을 다시 찾기 위한 **hyperlinked study map**입니다.
위에서 원하는 주제를 클릭하면 해당 설명, PDF 원자료, 실습 노트북으로 바로 이동할 수 있게 구성했습니다.

## Quick Table of Contents

- [Study Roadmap](#study-roadmap)
- [Repository Structure](#repository-structure)
- [Subject Index](#subject-index)
- [Environment](#environment)
- [Learning Sources](#learning-sources)
- [NumPy Basics](#numpy-basics)
- [Array Creation](#array-creation)
- [Shape Axis and Broadcasting](#shape-axis-and-broadcasting)
- [Indexing and Slicing](#indexing-and-slicing)
- [Array Methods and Reshape](#array-methods-and-reshape)
- [Random and Statistics](#random-and-statistics)
- [Vectorization Reduction and Linear Algebra](#vectorization-reduction-and-linear-algebra)
- [Array Combining](#array-combining)
- [Matplotlib Basics](#matplotlib-basics)
- [Figure Axes and Subplots](#figure-axes-and-subplots)
- [Chart Types](#chart-types)
- [Distribution Visualization](#distribution-visualization)
- [Graph Styling and Export](#graph-styling-and-export)
- [Pandas Basics](#pandas-basics)
- [Series DataFrame and Missing Values](#series-dataframe-and-missing-values)
- [CSV and DataFrame Structure](#csv-and-dataframe-structure)
- [Pandas Indexing and Selection](#pandas-indexing-and-selection)
- [Data Cleaning and Missing Data](#data-cleaning-and-missing-data)
- [DatetimeIndex Grouping and Filtering](#datetimeindex-grouping-and-filtering)
- [Pivot Concat and Merge](#pivot-concat-and-merge)
- [Practice Notebook](#practice-notebook)
- [More Study Topics](#more-study-topics)
- [README Maintenance Notes](#readme-maintenance-notes)

## Study Roadmap

이 저장소는 아래 흐름으로 공부하면 좋습니다.

| Step | Topic | Main file | Goal |
| --- | --- | --- | --- |
| 1 | NumPy가 필요한 이유 | [`1_넘파이_KarL.pdf`](1_%EB%84%98%ED%8C%8C%EC%9D%B4_KarL.pdf) | Python list와 `ndarray`의 차이를 이해합니다. |
| 2 | 배열 생성과 속성 | [`numpy/ex_01.ipynb`](numpy/ex_01.ipynb) | `array`, `zeros`, `ones`, `eye`, `arange`, `linspace`를 연습합니다. |
| 3 | shape, axis, broadcasting | [`1_넘파이_KarL.pdf`](1_%EB%84%98%ED%8C%8C%EC%9D%B4_KarL.pdf) | 다차원 배열의 축 방향과 자동 확장 규칙을 이해합니다. |
| 4 | indexing, slicing, logical indexing | [`numpy/ex_01.ipynb`](numpy/ex_01.ipynb) | 필요한 행, 열, 조건에 맞는 값만 뽑아냅니다. |
| 5 | 통계와 난수 | [`1_넘파이_KarL.pdf`](1_%EB%84%98%ED%8C%8C%EC%9D%B4_KarL.pdf) | 평균, 분산, 표준편차, 난수, 정규분포 데이터를 다룹니다. |
| 6 | Matplotlib 기본 그래프 | [`2_맷플롯립_KarL.pdf`](2_%EB%A7%B7%ED%94%8C%EB%A1%AF%EB%A6%BD_KarL.pdf) | `plot`, `xlabel`, `ylabel`, `title`, `legend`를 사용합니다. |
| 7 | 여러 그래프와 다양한 차트 | [`numpy/ex_01.ipynb`](numpy/ex_01.ipynb) | subplot, scatter, bar, pie, heatmap, histogram, box plot을 비교합니다. |
| 8 | Pandas 기본 자료구조 | [`4_팬다스_KarL.pdf`](4_%ED%8C%AC%EB%8B%A4%EC%8A%A4_KarL.pdf) | `Series`와 `DataFrame`으로 표 데이터를 표현합니다. |
| 9 | CSV, 결측값, 시계열 | [`4_팬다스_KarL.pdf`](4_%ED%8C%AC%EB%8B%A4%EC%8A%A4_KarL.pdf) | `read_csv`, `describe`, `isna`, `fillna`, `DatetimeIndex`를 익힙니다. |
| 10 | 그룹핑과 테이블 결합 | [`4_팬다스_KarL.pdf`](4_%ED%8C%AC%EB%8B%A4%EC%8A%A4_KarL.pdf) | `groupby`, filtering, `pivot`, `concat`, `merge`를 정리합니다. |

## Repository Structure

| Path | Purpose |
| --- | --- |
| [`README.md`](README.md) | NumPy와 Matplotlib 학습 내용을 주제별로 다시 찾기 위한 학습노트입니다. |
| [`1_넘파이_KarL.pdf`](1_%EB%84%98%ED%8C%8C%EC%9D%B4_KarL.pdf) | NumPy의 배열, 브로드캐스팅, 인덱싱, 난수, 통계, 벡터화, 선형대수 학습 자료입니다. |
| [`2_맷플롯립_KarL.pdf`](2_%EB%A7%B7%ED%94%8C%EB%A1%AF%EB%A6%BD_KarL.pdf) | Matplotlib의 선 그래프, subplot, 산점도, 막대 그래프, 히스토그램, 상자 그림 학습 자료입니다. |
| [`4_팬다스_KarL.pdf`](4_%ED%8C%AC%EB%8B%A4%EC%8A%A4_KarL.pdf) | Pandas의 Series, DataFrame, CSV, 결측값 처리, 시계열, 그룹핑, pivot, concat, merge 학습 자료입니다. |
| [`numpy/ex_01.ipynb`](numpy/ex_01.ipynb) | PDF 내용을 직접 실행해 보는 NumPy와 Matplotlib 실습 노트북입니다. |
| [`numpy/Sine-Cosine.pdf`](numpy/Sine-Cosine.pdf) | sin, cos 그래프 저장 결과로 보이는 PDF 출력물입니다. |
| [`pyproject.toml`](pyproject.toml) | Python 버전과 `numpy`, `matplotlib`, `ipykernel` 의존성을 기록한 프로젝트 설정입니다. |

생성 파일은 학습 대상이 아닙니다. 예를 들어 `.venv/`, `.idea/`, `__pycache__/`, 임시 추출 파일은 실행 또는 도구 사용 중 만들어지는 결과물이므로 README의 주요 학습 파일로 다루지 않습니다.

## Subject Index

| Subject | Files | What to study |
| --- | --- | --- |
| [Environment](#environment) | [`pyproject.toml`](pyproject.toml) | Python version, virtual environment, Jupyter kernel |
| [Learning Sources](#learning-sources) | [`1_넘파이_KarL.pdf`](1_%EB%84%98%ED%8C%8C%EC%9D%B4_KarL.pdf), [`2_맷플롯립_KarL.pdf`](2_%EB%A7%B7%ED%94%8C%EB%A1%AF%EB%A6%BD_KarL.pdf), [`4_팬다스_KarL.pdf`](4_%ED%8C%AC%EB%8B%A4%EC%8A%A4_KarL.pdf) | PDF별 학습 범위 |
| [NumPy Basics](#numpy-basics) | [`numpy/ex_01.ipynb`](numpy/ex_01.ipynb) | list와 `ndarray`, element-wise operation |
| [Array Creation](#array-creation) | [`numpy/ex_01.ipynb`](numpy/ex_01.ipynb) | `array`, `zeros`, `ones`, `full`, `eye`, `arange`, `linspace`, `logspace` |
| [Shape Axis and Broadcasting](#shape-axis-and-broadcasting) | [`1_넘파이_KarL.pdf`](1_%EB%84%98%ED%8C%8C%EC%9D%B4_KarL.pdf) | `shape`, `axis`, scalar broadcasting, vectorized operation |
| [Indexing and Slicing](#indexing-and-slicing) | [`numpy/ex_01.ipynb`](numpy/ex_01.ipynb) | 2D indexing, slicing, boolean mask |
| [Array Methods and Reshape](#array-methods-and-reshape) | [`1_넘파이_KarL.pdf`](1_%EB%84%98%ED%8C%8C%EC%9D%B4_KarL.pdf) | `max`, `min`, `mean`, `sort`, `astype`, `flatten`, `reshape` |
| [Random and Statistics](#random-and-statistics) | [`numpy/ex_01.ipynb`](numpy/ex_01.ipynb) | seed, random data, mean, variance, standard deviation |
| [Vectorization Reduction and Linear Algebra](#vectorization-reduction-and-linear-algebra) | [`1_넘파이_KarL.pdf`](1_%EB%84%98%ED%8C%8C%EC%9D%B4_KarL.pdf) | vectorization, reduction, `numpy.linalg` |
| [Array Combining](#array-combining) | [`1_넘파이_KarL.pdf`](1_%EB%84%98%ED%8C%8C%EC%9D%B4_KarL.pdf) | `concatenate`, `vstack`, `hstack`, `r_`, `c_`, `column_stack` |
| [Matplotlib Basics](#matplotlib-basics) | [`2_맷플롯립_KarL.pdf`](2_%EB%A7%B7%ED%94%8C%EB%A1%AF%EB%A6%BD_KarL.pdf) | `pyplot`, `plot`, `show`, axis range |
| [Figure Axes and Subplots](#figure-axes-and-subplots) | [`numpy/ex_01.ipynb`](numpy/ex_01.ipynb) | `Figure`, `Axes`, `Axis`, `subplots`, `GridSpec` |
| [Chart Types](#chart-types) | [`2_맷플롯립_KarL.pdf`](2_%EB%A7%B7%ED%94%8C%EB%A1%AF%EB%A6%BD_KarL.pdf) | line, scatter, bar, pie, heatmap |
| [Distribution Visualization](#distribution-visualization) | [`2_맷플롯립_KarL.pdf`](2_%EB%A7%B7%ED%94%8C%EB%A1%AF%EB%A6%BD_KarL.pdf) | histogram, normal distribution, density, box plot |
| [Graph Styling and Export](#graph-styling-and-export) | [`numpy/Sine-Cosine.pdf`](numpy/Sine-Cosine.pdf) | style, label, legend, grid, `savefig` |
| [Pandas Basics](#pandas-basics) | [`4_팬다스_KarL.pdf`](4_%ED%8C%AC%EB%8B%A4%EC%8A%A4_KarL.pdf) | Excel과 Pandas, table data, NumPy와 Pandas 관계 |
| [Series DataFrame and Missing Values](#series-dataframe-and-missing-values) | [`4_팬다스_KarL.pdf`](4_%ED%8C%AC%EB%8B%A4%EC%8A%A4_KarL.pdf) | `Series`, `DataFrame`, index, missing value, `isna` |
| [CSV and DataFrame Structure](#csv-and-dataframe-structure) | [`4_팬다스_KarL.pdf`](4_%ED%8C%AC%EB%8B%A4%EC%8A%A4_KarL.pdf) | `read_csv`, `index_col`, `columns`, `index`, new column |
| [Pandas Indexing and Selection](#pandas-indexing-and-selection) | [`4_팬다스_KarL.pdf`](4_%ED%8C%AC%EB%8B%A4%EC%8A%A4_KarL.pdf) | `head`, `tail`, slicing, `loc`, `iloc` |
| [Data Cleaning and Missing Data](#data-cleaning-and-missing-data) | [`4_팬다스_KarL.pdf`](4_%ED%8C%AC%EB%8B%A4%EC%8A%A4_KarL.pdf) | `describe`, `count`, `isna().sum`, `dropna`, `fillna` |
| [DatetimeIndex Grouping and Filtering](#datetimeindex-grouping-and-filtering) | [`4_팬다스_KarL.pdf`](4_%ED%8C%AC%EB%8B%A4%EC%8A%A4_KarL.pdf) | `DatetimeIndex`, `groupby`, `mean`, `max`, boolean filtering |
| [Pivot Concat and Merge](#pivot-concat-and-merge) | [`4_팬다스_KarL.pdf`](4_%ED%8C%AC%EB%8B%A4%EC%8A%A4_KarL.pdf) | `pivot`, `pivot_table`, `concat`, `merge`, `how`, `on` |

## Environment

이 저장소는 Python 기반의 수치 계산과 시각화 학습 저장소입니다. 현재 프로젝트 설정은 [`pyproject.toml`](pyproject.toml)에 기록되어 있습니다.

주요 의존성:

- `numpy`: 다차원 배열과 수치 계산
- `matplotlib`: 데이터 시각화
- `ipykernel`: Jupyter notebook 실행 커널

Pandas PDF를 실습하려면 `pandas`도 필요합니다. 현재 [`pyproject.toml`](pyproject.toml)에는 `numpy`, `matplotlib`, `ipykernel` 중심으로 기록되어 있으므로, Pandas 실습 파일을 추가할 때는 프로젝트 의존성에 `pandas`를 함께 추가하는 것이 좋습니다.

실행할 때 확인할 점:

- 같은 노트북이어도 어떤 Python interpreter를 쓰는지에 따라 import 결과가 달라질 수 있습니다.
- 가장 확실한 확인은 `python -c "import sys; print(sys.executable)"`입니다.
- Jupyter에서 실행한다면 현재 노트북 커널이 이 프로젝트의 `.venv`를 바라보는지 확인해야 합니다.
- Matplotlib 그래프는 Jupyter 환경에서는 자동 표시될 수 있지만, 일반 Python 파일에서는 보통 `plt.show()`가 필요합니다.

## Learning Sources

이 README는 아래 세 PDF의 학습 내용을 중심으로 정리했습니다.

| Source | Pages | Main topics |
| --- | --- | --- |
| [`1_넘파이_KarL.pdf`](1_%EB%84%98%ED%8C%8C%EC%9D%B4_KarL.pdf) | 102 pages | Python list와 NumPy 차이, `ndarray`, 브로드캐스팅, 배열 생성, 축, 삽입, 인덱싱, 논리 인덱싱, 정렬, reshape, 난수, 통계, 벡터화, 리덕션, 선형방정식, 배열 결합 |
| [`2_맷플롯립_KarL.pdf`](2_%EB%A7%B7%ED%94%8C%EB%A1%AF%EB%A6%BD_KarL.pdf) | 62 pages | 데이터 시각화 필요성, `pyplot`, 선 그래프, 저장, 제목, 레이블, 범례, 스타일, figure/axes, subplot, 산점도, 막대 그래프, 파이 차트, 히트맵, 히스토그램, 정규분포, box plot, grid |
| [`4_팬다스_KarL.pdf`](4_%ED%8C%AC%EB%8B%A4%EC%8A%A4_KarL.pdf) | 82 pages | Excel보다 강력한 table data 처리, `Series`, `DataFrame`, CSV, index/columns, 새 열 생성, `inplace`, DataFrame plot, `loc`, `iloc`, `describe`, 결측값 처리, `DatetimeIndex`, `groupby`, filtering, `pivot`, `concat`, `merge` |

## NumPy Basics

NumPy는 데이터 과학에서 가장 기본이 되는 수치 계산 라이브러리입니다. 핵심 자료구조는 `ndarray`입니다.

Python list와 NumPy array의 차이:

| 구분 | Python list | NumPy `ndarray` |
| --- | --- | --- |
| 자료형 | 서로 다른 자료형을 섞어 담을 수 있음 | 보통 같은 자료형의 값들을 연속적으로 저장 |
| 덧셈 | 두 list를 연결함 | 같은 위치의 원소끼리 더함 |
| 계산 관점 | 값들의 나열 | 벡터와 행렬 |
| 속도 | 큰 수치 데이터에서는 느릴 수 있음 | 대용량 배열과 행렬 연산에 적합 |

중요한 사고방식:

- NumPy 배열은 값을 단순히 보관하는 list가 아니라 계산 가능한 벡터로 생각해야 합니다.
- `a + b`, `a * b`, `a / b`는 대응되는 원소끼리 계산됩니다.
- `ndarray`는 `shape`, `dtype`, `ndim`, `size` 같은 속성으로 배열의 상태를 확인할 수 있습니다.

예시:

```python
import numpy as np

store_a = np.array([10, 20, 30])
store_b = np.array([1, 2, 3])

print(store_a + store_b)  # [11 22 33]
```

## Array Creation

NumPy 배열은 직접 값을 넣어서 만들 수도 있고, 일정한 규칙으로 생성할 수도 있습니다.

기본 생성 함수:

| Function | Meaning |
| --- | --- |
| `np.array([...])` | Python list를 NumPy 배열로 변환합니다. |
| `np.zeros((n, m))` | 모든 값이 0인 배열을 만듭니다. |
| `np.ones((n, m))` | 모든 값이 1인 배열을 만듭니다. |
| `np.full((n, m), x)` | 모든 값이 `x`인 배열을 만듭니다. |
| `np.eye(n)` | 대각선이 1인 단위행렬을 만듭니다. |
| `np.arange(start, stop, step)` | 일정 간격의 값을 만듭니다. |
| `np.linspace(start, stop, count)` | 시작과 끝을 포함해 같은 간격의 값을 `count`개 만듭니다. |
| `np.logspace(x, y, count)` | `10**x`부터 `10**y`까지 로그 스케일의 값을 만듭니다. |

공부 포인트:

- `arange()`는 Python의 `range()`와 비슷하지만 실수 간격도 사용할 수 있습니다.
- `linspace()`는 그래프 x축처럼 일정 개수의 점이 필요할 때 자주 사용합니다.
- `logspace()`는 값의 크기가 1, 10, 100, 1000처럼 지수적으로 커지는 데이터를 만들 때 유용합니다.

예시:

```python
import numpy as np

x = np.linspace(0, np.pi, 11)
print(np.sin(x))
```

## Shape Axis and Broadcasting

NumPy를 제대로 이해하려면 `shape`과 `axis`를 먼저 잡아야 합니다.

핵심 개념:

- `shape`: 배열의 형태입니다. 예를 들어 `(2, 3)`은 2행 3열입니다.
- `axis`: 배열의 축입니다. 2차원 배열에서 `axis=0`은 행 방향, `axis=1`은 열 방향으로 이해하면 좋습니다.
- `(3,)`, `(1, 3)`, `(3, 1)`은 서로 다릅니다. 첫 번째는 1차원 배열이고, 나머지는 2차원 배열입니다.

Broadcasting은 크기가 다른 배열을 계산할 때 NumPy가 자동으로 형태를 맞춰 주는 규칙입니다.

예시:

```python
import numpy as np

a = np.array([10, 20, 30])
print(a * 10)  # [100 200 300]

b = np.array([[10, 20, 30], [40, 50, 60]])
c = np.array([2, 3, 4])
print(b + c)
```

위 예시에서 `c`는 각 행에 맞춰 확장된 것처럼 계산됩니다. 이처럼 하나의 명령을 여러 데이터에 한꺼번에 적용하는 방식을 벡터화 연산이라고도 합니다.

## Indexing and Slicing

NumPy 배열은 list처럼 index와 slice를 사용할 수 있지만, 다차원 배열에서는 각 축에 대해 동시에 범위를 지정할 수 있습니다.

기본 형태:

```python
import numpy as np

a = np.array([
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9],
])

print(a[0, 0])    # 1
print(a[1])       # [4 5 6]
print(a[:, 1])    # [2 5 8]
print(a[0:2, 1:3])
```

공부 포인트:

- `a[row, col]`처럼 행과 열을 동시에 지정할 수 있습니다.
- `a[:, 1]`은 모든 행에서 두 번째 열만 가져옵니다.
- `a[0:2, 1:3]`은 2차원 배열 안에서 작은 행렬을 잘라내는 느낌으로 이해하면 좋습니다.

논리 인덱싱:

```python
x = np.arange(1, 17).reshape(4, 4)
mask = x % 2 == 0

print(mask)
print(x[mask])
```

조건식을 배열에 적용하면 같은 shape의 boolean 배열이 만들어지고, 그 boolean 배열을 index로 사용하면 조건을 만족하는 값만 추출됩니다.

## Array Methods and Reshape

NumPy 배열은 데이터 분석에서 자주 쓰는 메서드와 변형 기능을 제공합니다.

자주 쓰는 기능:

| Function or method | Meaning |
| --- | --- |
| `max()` | 최댓값 |
| `min()` | 최솟값 |
| `mean()` | 평균 |
| `std()` | 표준편차 |
| `sort()` | 정렬 |
| `astype(type)` | 자료형 변환 |
| `.T` | 전치 행렬 |
| `flatten()` | 2차원 이상 배열을 1차원으로 평탄화 |
| `reshape(...)` | 원소 개수는 유지하고 배열 형태를 변경 |

`reshape()`에서 가장 중요한 규칙:

- 원소 개수는 바뀌지 않습니다.
- `np.arange(12).reshape(3, 4)`는 가능하지만, 원소 12개를 `(5, 5)`로 바꿀 수는 없습니다.
- `-1`을 넣으면 나머지 차원을 기준으로 자동 계산됩니다.

예시:

```python
import numpy as np

a = np.arange(1, 13)
print(a.reshape(3, 4))
print(a.reshape(2, -1))
```

## Random and Statistics

데이터 과학에서는 실제 데이터를 수집하기 전, 비슷한 성질을 가진 가상 데이터를 만들어 실험하는 경우가 많습니다. 이때 난수와 통계 개념이 필요합니다.

난수 관련 개념:

- 컴퓨터가 만드는 난수는 보통 완전한 무작위가 아니라 의사 난수입니다.
- `seed`를 고정하면 같은 난수열을 다시 얻을 수 있습니다.
- 실험 결과를 재현하려면 seed를 명시하는 습관이 좋습니다.

자주 쓰는 함수:

| Function | Meaning |
| --- | --- |
| `np.random.randint(low, high, size)` | 정수 난수 |
| `np.random.rand(...)` | 0 이상 1 미만의 균등분포 난수 |
| `np.random.randn(...)` | 표준 정규분포 난수 |
| `np.random.normal(loc, scale, size)` | 평균과 표준편차를 지정한 정규분포 난수 |
| `np.random.seed(n)` | 난수 seed 고정 |
| `np.random.shuffle(arr)` | 원본 배열을 직접 섞음 |
| `np.random.permutation(arr)` | 섞인 새 배열을 반환 |

평균, 분산, 표준편차:

- 평균은 데이터의 대표값입니다.
- 분산은 값들이 평균에서 얼마나 퍼져 있는지를 나타냅니다.
- 표준편차는 분산에 제곱근을 씌운 값이라 원래 데이터 단위와 비교하기 쉽습니다.

예시:

```python
import numpy as np

np.random.seed(42)
heights = np.random.normal(loc=165, scale=10, size=10)

print(heights.mean())
print(heights.var())
print(heights.std())
```

## Vectorization Reduction and Linear Algebra

NumPy가 성공한 큰 이유는 배열 프로그래밍과 벡터화 연산입니다.

벡터화 연산:

- 반복문으로 원소를 하나씩 처리하지 않고 배열 전체에 연산을 적용합니다.
- 코드가 짧아지고, 큰 배열에서는 실행 속도도 크게 좋아집니다.
- PDF 자료에서는 배열 크기가 커질수록 반복문 방식보다 벡터화 연산이 훨씬 빠르다는 점을 성능 측정으로 설명합니다.

예시:

```python
import numpy as np

a = np.random.rand(100000)
b = np.random.rand(100000)

result = a * b
```

Reduction은 여러 값을 하나의 값으로 집계하는 기능입니다.

대표 함수:

- `np.sum(arr)`
- `np.mean(arr)`
- `np.min(arr)`
- `np.max(arr)`

축을 지정하면 전체 집계가 아니라 행 방향 또는 열 방향 집계를 할 수 있습니다.

```python
a = np.array([[1, 2, 3], [4, 5, 6]])

print(np.sum(a))          # 전체 합
print(np.sum(a, axis=0))  # 열 방향 집계
print(np.sum(a, axis=1))  # 행 방향 집계
```

선형대수:

NumPy는 `numpy.linalg` 서브 모듈로 선형방정식 풀이 같은 기능을 제공합니다.

```python
import numpy as np

A = np.array([[1, 1, -1], [2, -1, 3], [1, 2, 1]], dtype="int32")
b = np.array([0, 9, 8])

x = np.linalg.solve(A, b)
print(x)
```

머신러닝과 딥러닝에서는 대부분의 데이터가 벡터와 행렬 형태로 표현되므로, NumPy의 선형대수 감각은 이후 학습의 기초가 됩니다.

## Array Combining

여러 배열을 붙이는 방법도 자주 사용됩니다.

| Function | Meaning |
| --- | --- |
| `np.concatenate([a, b])` | 배열을 지정한 축 방향으로 연결합니다. |
| `np.vstack([a, b])` | 위아래로 쌓습니다. |
| `np.hstack([a, b])` | 좌우로 붙입니다. |
| `np.r_[a, b]` | 행 방향으로 쉽게 연결합니다. |
| `np.c_[a, b]` | 열 방향으로 쉽게 연결합니다. |
| `np.column_stack([a, b])` | 1차원 배열들을 열로 세워 2차원 배열을 만듭니다. |

주의할 점:

- 연결하려는 축이 아닌 나머지 차원의 크기는 서로 맞아야 합니다.
- 1차원 배열을 붙일 때와 2차원 배열을 붙일 때 결과 shape이 달라질 수 있습니다.
- `axis`를 명시하지 않으면 의도와 다르게 1차원으로 펴져 붙는 경우가 있습니다.

## Matplotlib Basics

Matplotlib은 Python에서 가장 널리 사용하는 시각화 도구 중 하나입니다. 이 저장소에서는 주로 `matplotlib.pyplot`을 `plt`라는 별칭으로 사용합니다.

기본 흐름:

```python
import matplotlib.pyplot as plt

plt.plot([1, 2, 3, 4])
plt.xlabel("x")
plt.ylabel("y")
plt.title("simple line")
plt.show()
```

핵심:

- `plt.plot([1, 2, 3, 4])`처럼 y 값만 주면 x 값은 0부터 자동으로 잡힙니다.
- x와 y를 모두 지정하려면 `plt.plot(x, y)` 형태를 사용합니다.
- `plt.axis([xmin, xmax, ymin, ymax])`로 축 범위를 직접 지정할 수 있습니다.
- NumPy 배열을 넘겨 그래프를 그리면 수학 함수 시각화가 쉬워집니다.

예시:

```python
import numpy as np
import matplotlib.pyplot as plt

x = np.arange(0, 10)
y = x ** 2

plt.plot(x, y)
plt.axis([0, 10, 0, 100])
plt.show()
```

## Figure Axes and Subplots

간단한 그래프는 `plt.plot()`만으로도 충분하지만, 여러 그래프를 한 화면에 배치하려면 `Figure`와 `Axes`를 이해해야 합니다.

구분:

| Name | Meaning |
| --- | --- |
| `Figure` | 전체 그림판입니다. 여러 Axes를 포함할 수 있습니다. |
| `Axes` | 실제 그래프가 그려지는 영역입니다. |
| `Axis` | x축, y축 같은 축 객체입니다. `Axes`와 헷갈리지 않아야 합니다. |

예시:

```python
import matplotlib.pyplot as plt

fig, ax = plt.subplots(2, 2)

ax[0, 0].plot([1, 2, 3])
ax[0, 1].bar(["A", "B"], [10, 20])
ax[1, 0].scatter([1, 2, 3], [3, 1, 2])
ax[1, 1].imshow([[1, 2], [3, 4]])

plt.show()
```

`GridSpec`은 subplot의 위치와 크기를 더 세밀하게 조절할 때 사용합니다. `wspace`, `hspace`는 subplot 사이의 가로, 세로 간격을 조절합니다.

## Chart Types

Matplotlib은 데이터 성격에 따라 여러 차트를 제공합니다.

| Chart | Function | Good for |
| --- | --- | --- |
| Line chart | `plot()` | 시간 흐름, 함수 그래프, 연속적인 변화 |
| Scatter plot | `scatter()` | 두 변수의 관계, 분포 |
| Bar chart | `bar()` | 범주별 값 비교 |
| Pie chart | `pie()` | 전체 중 각 범주의 비율 |
| Heatmap | `imshow()` | 행렬 데이터의 값 크기 분포 |

산점도:

```python
import numpy as np
import matplotlib.pyplot as plt

x = np.random.rand(100)
y = np.random.rand(100)
size = (30 * np.random.rand(100)) ** 2

plt.scatter(x, y, s=size, alpha=0.5)
plt.show()
```

막대 그래프:

```python
years = ["2024", "2025", "2026"]
values = [10, 15, 13]

plt.bar(years, values, width=0.5)
plt.show()
```

히트맵:

```python
data = np.random.rand(10, 10)

plt.imshow(data, cmap="cool")
plt.colorbar()
plt.show()
```

## Distribution Visualization

데이터 분석에서는 단순히 값 하나를 보는 것보다, 값들이 어떻게 퍼져 있는지 보는 일이 중요합니다.

### Histogram

히스토그램은 데이터를 여러 구간으로 나누고, 각 구간에 데이터가 몇 개 들어가는지 보여줍니다.

```python
import numpy as np
import matplotlib.pyplot as plt

heights = np.random.normal(loc=165, scale=10, size=1000)

plt.hist(heights, bins=20)
plt.show()
```

공부 포인트:

- `bins`가 너무 작으면 분포가 뭉개져 보입니다.
- `bins`가 너무 크면 분포가 지나치게 잘게 쪼개져 흐름을 보기 어렵습니다.
- `density=True`를 사용하면 막대의 개수가 아니라 확률 밀도 형태로 정규화됩니다.

### Normal Distribution

정규분포는 평균 근처가 가장 높고 좌우로 갈수록 낮아지는 종 모양의 연속 확률 분포입니다.

NumPy에서는 `np.random.normal(loc, scale, size)`로 평균과 표준편차를 지정한 정규분포 데이터를 만들 수 있습니다.

Matplotlib에서는 히스토그램으로 표본 분포를 그리고, 필요하면 확률 밀도 함수 곡선을 함께 그려 분포를 확인합니다.

### Box Plot

상자 수염 그림은 데이터의 중앙값, 사분위수, 범위, 이상치를 한 번에 보기 위한 그래프입니다.

핵심 용어:

- `Q1`: 하위 25% 지점
- `Q2`: 중앙값
- `Q3`: 상위 25% 지점
- `IQR`: `Q3 - Q1`
- Whisker: 대부분의 데이터가 분포하는 범위
- Outlier: 일반적인 범위에서 벗어난 값

```python
data = [
    np.random.normal(0, 1, 100),
    np.random.normal(3, 1, 100),
    np.random.normal(0, 3, 100),
]

plt.boxplot(data)
plt.show()
```

## Graph Styling and Export

그래프는 데이터만 맞다고 끝나는 것이 아니라, 읽는 사람이 의미를 쉽게 이해할 수 있어야 합니다.

자주 쓰는 꾸미기 함수:

| Function | Meaning |
| --- | --- |
| `plt.title(...)` | 그래프 제목 |
| `plt.xlabel(...)` | x축 레이블 |
| `plt.ylabel(...)` | y축 레이블 |
| `plt.legend(...)` | 범례 |
| `plt.grid(...)` | 격자 |
| `plt.style.use(...)` | 스타일시트 적용 |
| `plt.figure(figsize=(w, h))` | 그림 크기 조절 |
| `fig.savefig(...)` | 파일로 저장 |

범례를 표시하려면 그래프를 그릴 때 `label`을 먼저 넣어야 합니다.

```python
import numpy as np
import matplotlib.pyplot as plt

x = np.linspace(0, 2 * np.pi, 1000)

fig = plt.figure(figsize=(8, 4))
plt.plot(x, np.sin(x), label="sin")
plt.plot(x, np.cos(x), label="cos")
plt.title("Sine and Cosine")
plt.xlabel("x")
plt.ylabel("value")
plt.legend()
plt.grid(color="gray", linestyle="--", linewidth=0.5)

fig.savefig("numpy/Sine-Cosine.pdf")
plt.show()
```

저장 가능한 형식은 PNG, JPG, SVG, TIF, PDF 등 다양합니다. PDF 자료에서는 `fig.canvas.get_supported_filetypes()`로 현재 환경에서 지원하는 저장 형식을 확인할 수 있다고 설명합니다.

## Pandas Basics

Pandas는 Excel처럼 행과 열로 된 표 데이터를 Python에서 다루기 위한 라이브러리입니다. NumPy가 같은 자료형의 수치 배열을 빠르게 처리하는 데 강하다면, Pandas는 서로 다른 자료형이 섞인 현실적인 테이블 데이터를 읽고, 고치고, 분석하는 데 강합니다.

Pandas가 필요한 이유:

- 데이터 과학에서 많이 쓰는 데이터는 2차원 표 형태입니다.
- 표 데이터에는 행 이름, 열 이름, 숫자, 문자열, 날짜, 결측값이 함께 들어갑니다.
- NumPy 배열은 빠르지만 열 이름과 데이터 의미를 함께 표현하기 어렵습니다.
- Pandas는 NumPy를 기반으로 하면서 `Series`와 `DataFrame`이라는 구조를 제공합니다.

Excel과 비교해서 생각하면 좋습니다.

| Excel | Pandas |
| --- | --- |
| 눈으로 직접 표를 편집 | 코드로 표를 재현 가능하게 처리 |
| 작은 데이터 확인에 편리 | 큰 데이터, 반복 작업, 자동 분석에 유리 |
| 셀 단위 조작 중심 | 열, 행, 조건, 그룹 단위 조작 중심 |
| 수작업 실수 가능 | 같은 코드로 같은 처리 반복 가능 |

기본 import:

```python
import pandas as pd
```

## Series DataFrame and Missing Values

Pandas의 기본 자료구조는 `Series`와 `DataFrame`입니다.

| Structure | Shape | Meaning |
| --- | --- | --- |
| `Series` | 1차원 | index가 붙은 하나의 열 |
| `DataFrame` | 2차원 | 여러 Series가 모인 표 |

`Series`는 index가 있는 1차원 배열입니다.

```python
import pandas as pd

income = pd.Series(
    [100, 120, 90, 140],
    index=["Jan", "Feb", "Mar", "Apr"],
)

print(income["Jan"])
print(income.mean())
```

`DataFrame`은 행과 열을 가진 2차원 표입니다.

```python
import pandas as pd

df = pd.DataFrame({
    "income": [100, 120, 90, 140],
    "expense": [70, 80, 60, 100],
}, index=["Jan", "Feb", "Mar", "Apr"])

df["profit"] = df["income"] - df["expense"]
print(df)
```

결측값:

- 실제 데이터에는 값이 비어 있는 경우가 많습니다.
- Pandas에서는 이런 값을 보통 `NaN`으로 표현합니다.
- 결측값 여부는 `isna()`로 확인합니다.

```python
print(df.isna())
print(df.isna().sum())
```

## CSV and DataFrame Structure

CSV는 comma separated values의 약자입니다. 쉼표로 열을 구분한 텍스트 파일이며, 표 데이터를 저장하고 교환할 때 자주 사용합니다.

Pandas에서 CSV 읽기:

```python
import pandas as pd

df = pd.read_csv("vehicle_prodct.csv")
```

첫 번째 열을 index로 쓰고 싶다면 `index_col`을 지정합니다.

```python
df = pd.read_csv("vehicle_prodct.csv", index_col=0)
```

한글 CSV라면 인코딩을 명시해야 할 수 있습니다.

```python
weather = pd.read_csv("weather.csv", encoding="CP949")
```

DataFrame 구조 확인:

| Attribute or method | Meaning |
| --- | --- |
| `df.shape` | 행과 열 개수 |
| `df.index` | 행 index |
| `df.columns` | 열 이름 |
| `df.dtypes` | 열별 자료형 |
| `df.head()` | 앞부분 일부 확인 |
| `df.tail()` | 뒷부분 일부 확인 |
| `df.describe()` | 수치형 열의 요약 통계 |

새 열 생성:

```python
year_cols = ["2007", "2008", "2009", "2010", "2011"]

df["total"] = df[year_cols].sum(axis=1)
df["average"] = df[year_cols].mean(axis=1)
```

여기서 `axis=1`은 각 행을 따라 열 값들을 계산한다는 의미입니다. 반대로 `axis=0`은 열 방향으로 행 값들을 집계합니다.

`inplace`:

- `inplace=True`는 기존 DataFrame 자체를 바꿉니다.
- `inplace=False` 또는 기본값은 바뀐 결과를 새 DataFrame으로 반환합니다.
- 학습 단계에서는 원본을 잃지 않도록 새 변수에 받는 방식이 더 안전합니다.

```python
new_df = df.drop("total", axis=1)
```

## Pandas Indexing and Selection

Pandas에서 데이터를 잘 고르려면 column 선택, row 선택, label 기반 선택, 위치 기반 선택을 구분해야 합니다.

자주 쓰는 선택 방법:

| Expression | Meaning |
| --- | --- |
| `df["col"]` | 특정 열 선택 |
| `df[["a", "b"]]` | 여러 열 선택 |
| `df.head()` | 앞 5행 |
| `df.tail()` | 뒤 5행 |
| `df[m:n]` | 위치 기준 행 slice |
| `df.loc["Korea"]` | label 기준 행 선택 |
| `df.loc["Korea", "2009"]` | label 기준 특정 값 선택 |
| `df.iloc[4]` | 정수 위치 기준 행 선택 |
| `df.iloc[0:3, 1:4]` | 정수 위치 기준 행/열 slice |

`loc`와 `iloc`의 차이:

- `loc`: label을 사용합니다. index 이름이나 column 이름으로 접근합니다.
- `iloc`: integer location을 사용합니다. 0부터 시작하는 위치 번호로 접근합니다.

예시:

```python
print(df.loc["Korea"])
print(df.loc[["US", "Korea"]])
print(df.loc["Korea", "2009"])

print(df.iloc[4])
print(df.iloc[0:3, 1:4])
```

주의할 점:

- `df.loc["US", "Korea"]`는 `US` 행과 `Korea` 열을 찾는 뜻이므로, 여러 행을 고르려면 `df.loc[["US", "Korea"]]`처럼 list를 사용해야 합니다.
- `iloc["Korea"]`처럼 label을 넣으면 오류가 납니다. `iloc`는 정수 위치만 받습니다.

## Data Cleaning and Missing Data

데이터 분석 전에는 데이터 정제가 필요합니다. 실제 데이터에는 누락값, 잘못된 형식, 불필요한 행과 열이 들어갈 수 있습니다.

요약 통계:

```python
print(weather.describe())
print(weather.mean(numeric_only=True))
print(weather.std(numeric_only=True))
```

`describe()`는 수치형 열의 `count`, `mean`, `std`, `min`, `max` 등을 한 번에 보여줍니다. 문자열 열은 기본 요약에서 빠질 수 있습니다.

결측값 확인:

```python
print(weather.isna())
print(weather.isna().sum())
print(weather.isna().sum().sum())
```

결측값 처리 방법:

| Method | Meaning | Caution |
| --- | --- | --- |
| `dropna()` | 결측값이 있는 행이나 열 제거 | 데이터가 많이 줄어들 수 있음 |
| `fillna(0)` | 결측값을 0으로 대체 | 평균 같은 통계를 왜곡할 수 있음 |
| `fillna(mean_value)` | 결측값을 평균으로 대체 | 단순하지만 자주 쓰는 방식 |
| `fillna(method="ffill")` | 직전 값으로 채움 | 시계열 데이터에서 유용 |
| `fillna(method="bfill")` | 직후 값으로 채움 | 다음 관측값을 사용할 때 유용 |

예시:

```python
wind_mean = weather["평균풍속"].mean()
weather["평균풍속"] = weather["평균풍속"].fillna(wind_mean)
```

결측값을 무조건 0으로 채우면 실제 평균이나 분포가 달라질 수 있습니다. 어떤 값으로 채울지는 데이터 의미를 보고 결정해야 합니다.

## DatetimeIndex Grouping and Filtering

시계열 데이터는 시간 순서대로 관측한 데이터입니다. 날씨 데이터처럼 날짜별로 기록된 자료를 다룰 때 Pandas의 날짜 처리 기능이 중요합니다.

날짜 변환:

```python
weather["일시"] = pd.to_datetime(weather["일시"])
weather["year"] = weather["일시"].dt.year
weather["month"] = weather["일시"].dt.month
weather["day"] = weather["일시"].dt.day
```

`DatetimeIndex` 또는 `datetime` column을 사용하면 연도, 월, 일, 시간 같은 값을 쉽게 뽑아낼 수 있습니다.

`groupby()`:

```python
monthly_means = weather.groupby("month").mean(numeric_only=True)
yearly_means = weather.groupby("year").mean(numeric_only=True)
yearly_max = weather.groupby("year").max(numeric_only=True)
```

공부 포인트:

- `groupby("month")`는 같은 월끼리 행을 묶습니다.
- 뒤에 `mean()`, `max()`, `sum()` 같은 집계 함수를 붙여 그룹별 결과를 만듭니다.
- 숫자가 아닌 열이 섞여 있으면 `numeric_only=True`가 필요할 수 있습니다.

Filtering:

```python
windy_months = monthly_means[monthly_means["평균풍속"] >= 4.0]
```

조건식을 DataFrame에 적용하면 boolean mask가 만들어지고, 이 mask를 다시 DataFrame에 넣으면 조건을 만족하는 행만 남습니다. NumPy의 논리 인덱싱과 같은 사고방식입니다.

## Pivot Concat and Merge

Pandas에서는 표의 구조를 바꾸거나 여러 표를 합치는 일이 자주 있습니다.

### `pivot()` and `pivot_table()`

`pivot()`은 행으로 있던 값을 열로 펼쳐 표 구조를 바꿉니다.

```python
pivoted = df.pivot(index="상품", columns="재질", values="가격")
pivoted = pivoted.fillna(0)
```

공부 포인트:

- `index`: 새 행 index가 될 열
- `columns`: 새 column이 될 열
- `values`: 표 안에 채울 값
- 존재하지 않는 조합은 `NaN`이 될 수 있으므로 `fillna()`로 처리할 수 있습니다.

`pivot_table()`은 `pivot()`보다 더 일반적입니다. index나 column 조합이 여러 개이거나, 같은 조합에 여러 값이 있어 집계가 필요한 경우에는 `pivot_table()`을 사용합니다.

### `concat()`

`concat()`은 여러 DataFrame을 이어 붙입니다.

```python
combined = pd.concat([df_1, df_2], axis=0)
```

핵심 인자:

| Argument | Meaning |
| --- | --- |
| `axis=0` | 행 방향으로 붙임 |
| `axis=1` | 열 방향으로 붙임 |
| `join="outer"` | 열 또는 index의 합집합을 사용 |
| `join="inner"` | 공통으로 있는 열 또는 index만 사용 |

### `merge()`

`merge()`는 key를 기준으로 두 DataFrame을 조인합니다.

```python
merged = df_1.merge(df_2, on="B", how="inner")
```

`how`의 의미:

| `how` | Meaning |
| --- | --- |
| `inner` | 양쪽에 모두 있는 key만 남김 |
| `left` | 왼쪽 DataFrame의 key를 기준으로 유지 |
| `right` | 오른쪽 DataFrame의 key를 기준으로 유지 |
| `outer` | 양쪽 key의 합집합을 유지 |

주의할 점:

- 같은 이름의 열이 양쪽 DataFrame에 있으면 `_x`, `_y` 같은 suffix가 붙을 수 있습니다.
- `merge()` 결과에서는 기존 index가 사라질 수 있습니다.
- index를 key로 병합하려면 `left_index=True`, `right_index=True` 같은 옵션을 사용할 수 있습니다.

## Practice Notebook

Related file:

- [`numpy/ex_01.ipynb`](numpy/ex_01.ipynb)

이 노트북은 NumPy와 Matplotlib PDF에서 배운 내용을 직접 실행해 보는 실습 파일입니다. Pandas PDF 내용은 아직 별도 노트북으로 정리되어 있지 않으므로, 이후 `pandas/` 폴더나 새 notebook을 만들어 실습을 이어가면 좋습니다.

현재 노트북에서 확인되는 주요 흐름:

1. Python list와 NumPy array 비교
2. `np.array`, `np.zeros`, `np.eye`
3. `range`, list comprehension, `np.linspace`
4. `np.sin`
5. `np.insert`, 2차원 배열 indexing
6. `reshape`, logical indexing
7. 정렬과 배열 복사
8. `train_test_split` 형태의 데이터 분리 연습
9. 난수와 정규분포 데이터
10. `np.linalg.solve`
11. Matplotlib `plot`
12. 2차 함수, 여러 선 스타일
13. sin/cos 그래프 저장
14. `subplots`, `GridSpec`
15. 막대 그래프와 정규분포 히스토그램

노트북을 공부할 때는 각 셀을 실행만 하지 말고, 출력 배열의 `shape`과 그래프의 x/y 축이 어떤 의미인지 같이 확인하는 것이 좋습니다.

## More Study Topics

다음 단계로 더 공부하면 좋은 주제입니다.

| Topic | Why it matters | Related section |
| --- | --- | --- |
| pandas 실습 노트북 | PDF 내용을 직접 실행하면서 표 데이터 처리 흐름을 익힙니다. | [Pandas Basics](#pandas-basics) |
| scikit-learn | 머신러닝 모델 학습과 평가에 자주 사용됩니다. | NumPy 배열 shape이 입력 데이터 구조가 됩니다. |
| broadcasting rules in detail | shape 오류를 줄이는 데 중요합니다. | [Shape Axis and Broadcasting](#shape-axis-and-broadcasting) |
| matrix multiplication | 딥러닝의 선형 계층과 직접 연결됩니다. | [Vectorization Reduction and Linear Algebra](#vectorization-reduction-and-linear-algebra) |
| probability distribution | 데이터 생성과 모델 해석에 필요합니다. | [Distribution Visualization](#distribution-visualization) |
| visualization design | 그래프를 정확하고 읽기 쉽게 만드는 능력입니다. | [Graph Styling and Export](#graph-styling-and-export) |

## README Maintenance Notes

새 학습 파일을 추가할 때는 아래 순서로 README도 같이 업데이트하면 찾기 쉽습니다.

1. [Repository Structure](#repository-structure)에 새 파일의 역할을 추가합니다.
2. [Subject Index](#subject-index)에 주제와 파일 링크를 추가합니다.
3. 관련 topic section의 설명이나 예시 코드를 보강합니다.
4. 실습 노트북을 추가했다면 [Practice Notebook](#practice-notebook)에 학습 흐름을 요약합니다.
5. 생성 파일, 가상환경, IDE 설정, 임시 파일은 주요 학습 목록에 넣지 않습니다.
