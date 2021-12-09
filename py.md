# Struct

struct Product {
    int weight;
    double price;
}

Product apple;
apple.price = 10;


Java
class Product{
    private int weight;
    private double price;
    
    public void setPrice(double Price){
        this.price = price;
    }
}

Product apple = new Product();
apple.setPrice(10);


Python
from collections import namedtuple
MyStruct = namedtuple("MyStruct", "Field1 Field2 Field3")
m = MyStruct("foo", "bar", "baz")

- 구조체 없음
- 클래스 데이터타입 지정 불가 -> namedtuple 사용

@dataclass decoration (java의 annotation)
!pop install dataclasses
from dataclasses import dataclass
@dataclass
class Product:
    weight: int = None
    price: float = None

apple = Product()
apple.price = 10

go

type Product struct{
    weight int
    price float64
}

var apple Product
apple.price = 10

TypeScript
interface Product{
    weight: number,
    price : number,
}
let apple = {} as Product;
apple.price = 10;


class Rectangle {
    int width, height;
public:
    Rectangle(int, int)    ;
    
    int area();
};

#config
Rectangle::Rectangle(int x, int y){
    width = x;
    height = y;
}

int Rectangle::area(){
    return width * height;
}

Rectangle rect(3,4);
std::cout << rect.area() << std.endl;

- 선언부와 구현부로 나눔 : 소스 파일, 헤더파일 
- 컴파일 속도 더 빠르게 할 수 있다는 장점

Java

class Rectangle {
    int width;
    int height;
    
    public Rectangle (int width, int height){
        this.width = width;
        this.height = height;
    }
    
    public int area(){
        return this.width * this.height;
    }
}

Rectangle rect = new Rectangle(3,4);
System.out.println(rect.area());

- 모든 것이 class

Python
from dataclasses import dataclass
@dataclass
class Rectangle:
    width : int 
    height : int
    
    def area(self):
        return self.width * self.height
        
rect= Rectangle(3,4)
print (rect.area())

- 내부 함수 기능 자동 구현 (dataclass)

go

type Geometry interface{
    area() int
}

type Rectangle struct{
    width int
    height int
}

func (r *Rectangle) area() int{
    return r.width * r.height
}

var rect Geometry = Rectangle{3,4}
fmt.PrintLn(rect.area())

- Polymorphism : 서로 다른 유형의 개체에 단일 인터페이스를ㅈ ㅔ공
- Geometry라는 단일 interface: 어떤 유형이냐에 따라 다양하게 구현



클로바 Vision/NLP 연구 개발 ▼
이런 일을 맡고 있어요
Visual AI팀은 네이버 클로바에서 Vision 및 NLP 기술을 담당하고 있는 조직으로 다음과 같은 기회를 가질 수 있습니다.
 - Computer vision 및 NLP 기술 전반에 대한 연구
 - OCR (Optical Character Recognition) 기술 및 문서 이미지 분석 기술 개발
 - Visual Information Extraction과 Semantic Parsing등 문서 인식 기술 개발
 - Multimodality를 기반한 대규모 Vision/NLP 사전 학습 모델 개발
 - 얼굴 검출 및 인식 관련 모델 및 디바이스 개발 참여
 - 비디오에서의 객체 추적, 행동인식, 3D 인식 모델 개발
 - ML기반 서비스를 위한 연구/개발 환경 및 프로세스의 표준화
 - Quantization, 경량화 등을 통해 AI모델이 실제 서비스에 적용되어 가는 과정 참여
 - Top-tier Vision/NLP/ML학회 paper 투고 지원
입사하게 되면 담당할 업무입니다
다양한 시각 데이터로부터 의미있는 정보를 추출하는 Vision 기술 연구 개발
이미지에서 문자의 검출/인식 및 문서의 구조/의미를 파악하는 기술 연구 개발
얼굴 검출, 인식 및 모델링 등의 AR 기술 연구 개발
비디오에서 이동 물체 추적 및 행동 분석 기술 개발
네이버 내 다양한 이미지/비디오에서 정보 추출을 위한 AI 모델 개발
Multimodal을 이용한 대규모의 이미지 사전학습 모델 개발
ML 기반 서비스 파이프라인 개발 (MLOps)
ML 모델의 경량화 및 Quantization을 통한 서비스 모델 개발
업무를 수행하기 위해 필요한 자격 요건입니다
컴퓨터과학, 컴퓨터엔지니어링, 수학 및 관련 분야 전공 (학사 이상)
ML resarcher/engineer/practitioner 역할 중 한가지 분야에서 1년 이상의 실무 경험을 보유
ML/DL에 분야에 대한 기본 지식
PyTorch나 Tensorflow와 같은 딥러닝프레임워크에 대한 지식 및 개발 경험
추가로 보유하고 있다면 좋을 스킬셋이나 경험입니다
Computer Vision 및 NLP top-tier 학회에 논문 게재 경험
Kaggle 등 머신러닝 챌린지 입상 경험
머신러닝을 활용한 서비스 경험
SW Engineering 기술 보유자
빅 모델 학습 경험 (multi-gpu/distributed training)
공유하기
http://www.naver-monthlyopening.com/#category-clova-ai-1
자연어 이해 및 대화 시스템 기술 개발 ▼
이런 일을 맡고 있어요
AI Assistant 조직은 Clova의 주요 제품인 AI 스피커의 대화 인터페이스를 개발하는 부서입니다. 사용자의 음성 언어 및 텍스트 입력을 컴퓨터가 이해할 수 있는 형태로 처리하는 자연어 이해, 그리고 현재 상황에 적합한 서비스 응답을 만들기 위한 대화 관리 등의 일련의 기술들을 개발하고 이를 실서비스에 적용하여 많은 사용자를 만나고 있습니다.
AI 스피커 뿐만 아니라 네이버 앱, 셋탑 박스, 네이버 지도/내비게이션의 음성 인터페이스에도 그 기술이 활용되고 있고, 한국을 넘어 일본에서도 사용자를 만나고 있습니다. 네이버가 가진 다양한 서비스를 음성과 대화로 사용자에게 연결하거나 음성 및 대화에 맞는 새로운 서비스를 개발하여 새로운 경험과 가치를 만들어 내는 것을 목표로 하고 있습니다.
입사하게 되면 담당할 업무입니다
입사하시면 네이버가 가지고 있는 수많은 데이터들을 활용해서 AI Assistant를 만드는 경험을 하실 수 있습니다.
내가 개발한 대화 시스템 기술이 네이버의 많은 사용자를 만나게 되는 경험을 하실 수 있습니다.
머신러닝, 자연어 처리를 위한 모델링에 일가견 있는 분들을 모십니다. 사용자의 발화를 잘 이해하고 좋은 응답을 내기 위한 자연어 이해 및 언어 모델 구축, e2e 언어 이해 및 대화 관리 기술, 음성 오류에 강인한 대화 관리 모델을 개발하게 됩니다
업무를 수행하기 위해 필요한 자격 요건입니다
주요 ML 프레임워크에 대한 이해가 깊은 분 (Tensorflow, pytorch 등)
문제 정의와 구현 능력이 뛰어난 분
하나 이상 프로그래밍 언어와 Linux/shell을 자유자재로 다루시는 분
자연어 처리 및 머신러닝에 조예가 깊으신 분
관련 분야에서 4년 이상 실무 경험을 보유하신 분 또는 자연어처리/머신러닝 기술로 석사/박사 학위를 가지신 분
Python, Go, C++ 등 하나 이상의 언어에 능숙하신 분
리눅스 환경에서의 개발에 익숙하신 분
추가로 보유하고 있다면 좋을 스킬셋이나 경험입니다
NLP나 NLU 관련 서비스 개발 및 운영 경험
머신러닝 기술이 적용된 서비스 개발 경험
대량의 데이터로 모델을 학습 및 평가해본 경험
ACL, EMNLP, AAAI, 등 자연어처리 및 대화 시스템 관련 학회 및 학회지에 논문 게재 경험
자연어 처리 관련한 challenge 나 shared task에서 입상 경험
NLP에 관련된 프로젝트 리딩 경험
일본어 회화/커뮤니케이션 능력
공유하기
http://www.naver-monthlyopening.com/#category-clova-ai-2
얼굴 및 모션합성 모델 개발 ▼
이런 일을 맡고 있어요
네이버 CLOVA의 Avatar 조직은 Virtual Avatar를 생성하는데 필요한 요소 기술을 연구 개발합니다.
사람의 얼굴(표정 및 입 모양) 및 모션을 생성하기도 하고 자세를 예측하기도 합니다. Avatar에 가치를 부여하고 싶으신 분들께서는 고민하지 마시고 지원해주세요!
입사하게 되면 담당할 업무입니다
Text와 Audio 정보를 기반으로 사람의 얼굴(표정, 입 모양) 및 모션을 생성하는 기술 개발
딥러닝 기반으로 얼굴 및 모션을 합성하는 모델(Model) 개발
업무를 수행하기 위해 필요한 자격 요건입니다
얼굴 및 모션합성 관련 경험을 보유하고 있는 분
PyTorch, TensorFlow 등 1개 이상의 프레임워크를 활용한 Model 개발 경험을 보유하고 있는 분
추가로 보유하고 있다면 좋을 스킬셋이나 경험입니다
Computer Vision 및 Graphics top-tier 학회에 논문 게재 경험이 있는 분
경령화 모델 개발 경험을 보유하고 있는 분
머신러닝을 활용한 서비스 개발 경험을 보유하고 있는 분
C/C++, Python 등 숙련된 개발 능력이 있는 분
공유하기
http://www.naver-monthlyopening.com/#category-clova-ai-3
음성합성 기술 개발▼
이런 일을 맡고 있어요
Clova 에 속한 Voice(음성 합성) 부서는 세계 최고 수준의 한국어, 일본어 음성 합성기를 보유하고 있으며, 다양한 분야의 전문가로부터 언어처리, 음성처리, Engineering 기술을 함께 배울 수 있는 조직입니다.
네이버의 목소리를 만드는 음성 합성팀에서 새로운 다국어 음성 합성기를 연구/개발할 인재를 찾고 있습니다.
자연어처리와 신호처리 두 분야의 지식을 함께 습득하며 세계 최고의 음성 합성기를 만들고 싶으신 분들의 많은 지원 부탁드립니다.
입사하게 되면 담당할 업무입니다
네이버 & 라인의 다국어 음성 합성기 개발을 담당합니다.
네이버 & 라인의 다국어 언어처리 모듈 개발을 담당합니다.
네이버 & 라인의 음성 합성, 자연어처리, 신호처리 연구를 담당합니다.
업무를 수행하기 위해 필요한 자격 요건입니다
음성신호처리 또는 자연어처리 관련 분야에서 2년 이상 실무 경험을 보유하고 있는 분
PyTorch, TensorFlow, Keras 등 하나 이상에 능숙하신 분
추가로 보유하고 있다면 좋을 스킬셋이나 경험입니다
음성 합성 모델 (Tacotron, Transformer 등) 개발 경험을 보유하고 있는 분
음성 합성 보코더 (WaveNet, WaveRNN, WaveGAN 등) 개발 경험을 보유하고 있는 분
다양한 환경에서의 개발 경험과 엔지니어링 능력을 보유하고 있는 분
최신 딥러닝 및 기계학습 모델링 기법을 활용한 서비스 개발 경험을 보유하고 있는 분
공유하기
http://www.naver-monthlyopening.com/#category-clova-ai-4
Healthcare AI 선행 연구 개발 ▼
이런 일을 맡고 있어요
Healthcare AI팀은 의료 및 건강 분야를 재정의할 수 있는 파괴적 혁신 기술 개발 및 현장 도입을 미션으로 합니다. 네이버의 다양한 생활 밀착형 서비스, 여러 의료 기관과의 협업을 통해 수많은 사람들의 건강에 직접적으로 기여할 수 있는 연구를 수행합니다.
AI 및 ML과 관련하여 깊이 있는 이론에서부터 응용 수준까지 폭넓게 다루고 있으며 의료 현장에서 사용할 수 있는 인공지능에서부터 네이버의 Healthcare 서비스의 핵심 AI 모델까지 다양한 연구/개발을 담당합니다. 이와 더불어 Healthcare AI 영역 내에서 글로벌 리더십 확보를 위해 국제적으로 impact가 큰 healthcare AI 학술 결과 창출을 책임집니다.
Healthcare AI팀에서는 풍부한 GPU 자원과 데이터, 다양한 의료 기관 및 뛰어난 동료들과의 협업을 통해 Healthcare AI 전문가로서 성장할 수 있습니다. 또한, 상위 부서인 AI Lab의 강력한 open innovation 정책에 따라 뛰어난 학계 대가들과 공동으로 활발한 연구를 진행하고 있습니다.
입사하게 되면 담당할 업무입니다
대용량 언어 모델을 이용한 Healthcare AI 모델 개발 - Patient representation learning, prediction, classification, QA, 요약 task 등
차세대 딥러닝 모델 구조 연구 - NAS, 모델 최적화, 모델 경량화, weak/self/semi-supervision, vision backbone model, optimization, 멀티모달 인식 등
HCI 연구 - Accessibility, Computational Interaction, Computational Social Science, 데이터 기반 interface 디자인, human computation, visualization 등
신뢰가능한 AI 연구 - Explanable AI, Causual inference, robustness, fair machine learning, 불확실성 추정, federated learning, differential privacy 등
Graph 구조 연구, time-series 데이터 연구
데이터 분석 - Healthcare 관련 서비스 데이터 분석, 공익 및 ESG를 위한 연구 등
업무를 수행하기 위해 필요한 자격 요건입니다
영향력 있는 AI 선행 연구를 해낼 수 있는 연구 능력
주도적으로 중장기 AI 연구 프로젝트를 이끌어나가고 협업할 수 있는 협업 능력
연구 코드를 빠르고 정확하게 작성할 수 있는 프로그래밍 스킬
추가로 보유하고 있다면 좋을 스킬셋이나 경험입니다
Healthcare 분야에 대한 연구 경험
CS, EE, mathematics 등의 분야의 PhD 혹은 그에 준하는 연구 업무 경력
활발한 연구 커뮤니티 경력 (reviewer, tutorial presenter, workshop organizer, open source 등)
다양한 open deep learning library (Pytorch, Tensorflow, MXNet 등) 이용 연구경험
공유하기
http://www.naver-monthlyopening.com/#category-clova-ai-5
중장기 AI 선행 연구 개발 ▼
이런 일을 맡고 있어요
NAVER AI LAB은 AI 기술 및 서비스의 패러다임을 바꿀 수 있는 혁신적인 중장기 선행 연구를 미션으로 합니다.
클로바, 네이버 검색, 네이버 랩스 등의 다양한 네이버의 AI 조직들과 협업해 서비스에 직접 기여할 수도 있으며, 공익을 위한 AI 혹은 신뢰가능한 AI와 같은 근본적인 문제에 대한 해결책도 고민합니다.

AI와 관련된 다양한 분야들 (기계학습, 컴퓨터 비전, 자연어 처리, 음성 인식, 음성 합성, HCI, 신뢰가능한 AI) 의 선행 기술 연구 개발을 수행하여 네이버 AI 역량 강화에 기여합니다. 네이버 AI 기술 조직에 AI tech transfer를 하거나, top-tier 학회에 논문을 발표하는 등의 역할을 합니다.
풍부한 GPU 및 데이터 자원들을 활용할 수 있으며, 뛰어난 AI 연구자들과 함께 연구하고 성장할 수 있습니다.
또한 국내외 연구역량이 뛰어난 대학들과 강한 협력연구를 수행하고 학생들을 함께 연구지도 합니다.
입사하게 되면 담당할 업무입니다
차세대 딥러닝 모델 구조 연구 - NAS, 모델 최적화, 모델 경량화, weak/self/semi-supervision, vision backbone model, optimization, 멀티모달 인식 등
Generative model 연구 - 이미지, 비디오, 텍스트, 오디오, cross-modal, image-to-image, video-to-video, disentanglement, style trasnfer, superresolution 등
대용량 언어 모델 (GPT-3 scale 이상) 연구 - controlled LM, 멀티모달, 대화, QA, 요약 task 등
HCI 연구 - Accessibility, Computational Interaction, Computational Social Science, 데이터 기반 interface 디자인, human computation, visualization 등
신뢰가능한 AI 연구 - Explanable AI, Causual inference, robustness, fair machine learning, 불확실성 추정, federated learning 등
Audio 인식/합성 연구 - 대규모 음성 인식 모델, 화자 분리 인식, 시각 기반 음성 인식, 음성합성, 음성스타일 변환, 음악인식/모델링/생성
Graph 구조 연구, time-series 데이터 연구, Reinforcement learning
헬스케어 연구, 공익 및 ESG를 위한 인공지능 연구
업무를 수행하기 위해 필요한 자격 요건입니다
영향력 있는 AI 선행 연구를 해낼 수 있는 연구 능력
주도적으로 중장기 AI 연구 프로젝트를 이끌어나가고 협업할 수 있는 협업 능력
연구 코드를 빠르고 정확하게 작성할 수 있는 프로그래밍 스킬
추가로 보유하고 있다면 좋을 스킬셋이나 경험입니다
CS, EE, mathematics 등의 분야의 PhD 혹은 그에 준하는 연구 업무 경력
활발한 연구 커뮤니티 경력 (reviewer, tutorial presenter, workshop organizer, open source 등)
다양한 open deep learning library (Pytorch, Tensorflow, MXNet 등) 이용 연구경험
공유하기
http://www.naver-monthlyopening.com/#category-clova-ai-6
모델 경량화/압축/최적화 기술 연구 및 개발 ▼
이런 일을 맡고 있어요
AI 모델의 본격적인 서비스 적용이 가시화됨에 따라 효율적인 Training/Inference에 대한 요구가 증가하고 있습니다.
빠르게 발전하는 CLOVA AI 서비스의 효용성을 높이기 위한 모델 경량화/압축/최적화 기술을 연구/개발합니다.
작은 모델부터 초거대 모델에 이르기까지 다양한 AI 모델을 위한 차별화된 Solution을 적용합니다. AI 모델 개발부터 서비스까지 폭넓은 경험을 하실 수 있습니다.
입사하게 되면 담당할 업무입니다
모델 경량화/압축/최적화 알고리즘 연구/개발
업무를 수행하기 위해 필요한 자격 요건입니다
PyTorch, TensorFlow 등을 사용한 모델 개발 역량
C/C++/CUDA 등을 이용한 low-level 라이브러리 개발
Machine learning 연구/개발 경력 1년 이상
추가로 보유하고 있다면 좋을 스킬셋이나 경험입니다
모델 경량화 관련 publication 경력
딥러닝 모델/서비스 개발/최적화 경력 혹은 하드웨어 설계 지식 보유
공유하기
http://www.naver-monthlyopening.com/#category-clova-ai-7
음성인식/자연어처리 엔진 개발 ▼
이런 일을 맡고 있어요
· 한국어 / 일본어 / 영어 음성 인식 & 언어 모델 연구 및 개발
· 텍스트를 분석하여, 사용자에게 도메인 분류, 중요 키워드, 요약 내용과 같은 유용한 정보를 제공해주는 NLP 연구 및 개발
입사하게 되면 담당할 업무입니다
음성인식 언어모델 및 클로바노트용 NLP 개발
업무를 수행하기 위해 필요한 자격 요건입니다
음성이나 자연어처리 혹은 언어모델 관련 각종 알고리즘에 대한 개발/서비스 경험이 있으신 분
딥러닝 모델링 기법을 활용한 서비스 개발 경험
Pytorch, Tensorflow 등 딥러닝 툴킷 사용에 익숙하신 분
공유하기
http://www.naver-monthlyopening.com/#category-clova-ai-8
언어 모델 연구 및 대화 시스템 개발 ▼
이런 일을 맡고 있어요
대화의 가치에 주목하고 자연어 관련 다양한 어플리케이션을 개발/서비스 하고 있습니다.
주요 서비스는 한국어/일본어 클로바 챗, 서드파티 사용자들을 위한 챗봇 빌더, AiCall /HappyCall 등 클로바 AI 고객센터 솔루션 등이 있습니다.
기계가 인간과 자연스러운 대화를 할 수 있는 데까지는 아직 풀리지 않은 문제가 많고 할 일도 산더미 같습니다.
어려운 문제에 도전하시는 걸 즐기시는 분, GPT-3 이상의 초대형 언어 모델을 학습해 보고 싶으신 분, 팀원들과 토론하고 아이디어를 발전시켜 나가는 걸 좋아하시는 분들은 주저 말고 문을 두드리세요!
입사하게 되면 담당할 업무입니다
초대형 언어 모델 연구 및 이를 위한 기계학습 프레임워크 구현
대화 모델을 위한 다양한 NLP 기술 및 딥러닝 모델 개발
목적 지향 대화 시스템(Task-Oriented Dialogue System) 연구 및 개발
질문답변(Question Answering), 문장 생성, 유사 문장 군집화(Clustering) 등 다양한 자연어 처리 연구 과제 수행
대화 데이터를 위한 Domain Adaptation / Semi-supervised Learning / Adversarial Training 에 대한 연구 및 개발
딥러닝 모델의 최적화, 경량화 연구 및 개발
텍스트, 이미지, 음성 등 멀티모달 입력에 대한 기계학습 모델 구축 및 서비스 적용
업무를 수행하기 위해 필요한 자격 요건입니다
Computer Science, Machine Learning, 수학/통계 관련 전공 석사 이상 학위 보유자 또는 이에 준하는 관련 프로젝트 경험 보유자
Python 및 딥러닝 프레임워크 (PyTorch, Tensorflow) 개발 역량
새로운 기술이나 업무에 대한 도전 정신
연구/개발에 대한 지속적인 관심
개인 역량 성장을 즐기는 태도
글로벌 시장에 대한 도전 의식
추가로 보유하고 있다면 좋을 스킬셋이나 경험입니다
자연어 처리 어플리케이션 혹은 언어/대화모델 개발 경험
텍스트, 음성 및 이미지 등을 활용한 멀티모달 모델 개발 경험
대형 딥러닝 모델 최적화, 분산 학습 개발 경험 (DeepSpeed, TensorRT 등)
CUDA 프로그래밍 및 슈퍼 컴퓨팅 개발 경험
ML 관련 주요 학회 및 저널 Publication 실적 (NeurIPS, ICML, ICLR, ACL, EMNLP, CVPR, ICCV, AAAI, IJCAI, KDD 등)
AI 관련 Challenge 수상 이력
공유하기
http://www.naver-monthlyopening.com/#category-clova-ai-9
LINE 추천 시스템 개발 ▼
이런 일을 맡고 있어요
네이버 및 라인의 비즈니스 지표 향상을 위해 AI를 적용하는 역할을 하고 있습니다. 최신 기계학습 방법론을 실제 비즈니스 문제에 적용하고 싶으신 마음이 있다면 현재 하고 있는 일이 무엇이든 도전해주세요.
실세계 데이터 분석, 기계학습 모델링, 모델성능의 실시간 평가 등 기계학습관련 전반적인 업무를 모두 경험하며 전문가로 성장할 수 있습니다.
역량있는 인재들이 함께 일하고 있으며 서로 성장에 도움을 주는 분위기를 구성하고 있습니다.
입사하게 되면 담당할 업무입니다
LINE (일본, 대만, 태국 등) 서비스를 위한 추천모델 개발
LINE 추천시스템의 운영
업무를 수행하기 위해 필요한 자격 요건입니다
PyTorch, TensorFlow 등 딥러닝프레임워크 중 하나 이상 구현 역량
Hive, Presto, Spark 등 빅데이터 질의처리 프레임워크 지식 및 사용 경험
머신러닝, 딥러닝 모델에 대한 기본 지식
최신 딥러닝 기술을 이해하고 구현가능하신 분
Python, SQL 언어에 능숙하신 분
추가로 보유하고 있다면 좋을 스킬셋이나 경험입니다
추천시스템 개발 및 운영 경험이 있으신 분
머신러닝을 서비스에 적용해본 경험이 있으신 분
NeurIPS, ICML, ICLR, KDD, WWW, AAAI 등 AI top-tier 컨퍼런스학회에 논문을 게재하신 분
공유하기
http://www.naver-monthlyopening.com/#category-clova-ai-10
쇼핑 AI 모델링 ▼
이런 일을 맡고 있어요
네이버 및 라인의 비즈니스 지표 향상을 위해 AI를 적용하는 역할을 하고 있습니다.
최신 기계학습 방법론을 실제 비즈니스 문제에 적용하고 싶으신 마음이 있다면 현재 하고 있는 일이 무엇이든 도전해주세요.
실세계 데이터 분석, 기계학습 모델링, 모델성능의 실시간 평가 등 기계학습관련 전반적인 업무를 모두 경험하며 전문가로 성장할 수 있습니다.
역량있는 인재들이 함께 일하고 있으며 서로 성장에 도움을 주는 분위기를 구성하고 있습니다.
입사하게 되면 담당할 업무입니다
하이퍼클로바를 활용한 차세대 쇼핑 AI 모델 개발
사용자에게 편리한 쇼핑 경험을 주기 위한 AI 모델 개발
판매자의 효율적인 업무를 위한 AI 모델 개발
추천시스템, 광고타게팅 AI 모델 개발
업무를 수행하기 위해 필요한 자격 요건입니다
머신러닝, 딥러닝 모델에 대한 기본 지식
최신 딥러닝 기술을 이해하고 구현가능
다양한 도메인의 pretrained model 사용 경험
협업 및 소통에 긍정적이고 적극적인 태도
추가로 보유하고 있다면 좋을 스킬셋이나 경험입니다
쇼핑 데이터를 다뤄보신 분
관련 있는 상품들을 자동으로 구성해본 경험이 있으신 분
머신러닝을 서비스에 적용해본 경험이 있으신 분
NeurIPS, ICML, ICLR, KDD, WWW, AAAI 등 AI top-tier 컨퍼런스학회에 논문을 게재하신 분
Kaggle 등 머신러닝 챌린지에서 입상하신 분
공유하기
http://www.naver-monthlyopening.com/#category-clova-ai-11
초대규모 멀티모달 모델링 연구 ▼
이런 일을 맡고 있어요
네이버 및 라인의 비즈니스 지표 향상을 위해 AI를 적용하는 역할을 하고 있습니다.
최신 기계학습 방법론을 실제 비즈니스 문제에 적용하고 싶으신 마음이 있다면 현재 하고 있는 일이 무엇이든 도전해주세요.
실세계 데이터 분석, 기계학습 모델링, 모델성능의 실시간 평가 등 기계학습관련 전반적인 업무를 모두 경험하며 전문가로 성장할 수 있습니다.
역량있는 인재들이 함께 일하고 있으며 서로 성장에 도움을 주는 분위기를 구성하고 있습니다.
입사하게 되면 담당할 업무입니다
대규모 네이버 멀티모달 데이터셋 제작 및 분석
머신러닝 및 딥러닝을 활용하여 멀티모달 예측모델링
초대형 클러스터를 사용한 예측모델 성능 최적화
딥러닝 모델의 분산처리 학습
업무를 수행하기 위해 필요한 자격 요건입니다
PyTorch, TensorFlow 등 딥러닝프레임워크 중 하나 이상 구현 역량
Hive, Presto, Spark 등 빅데이터 질의처리 프레임워크 지식 및 사용 경험
객체지향 개발, 리팩토링, 자동화 테스트에 대한 기본 지식
머신러닝, 딥러닝 모델에 대한 기본 지식
최신 딥러닝 기술을 이해하고 구현가능하신 분
Python, SQL 언어에 능숙하신 분
빅데이터 처리 프레임워크(ex> Hadoop)에 대한 이해가 깊으신 분
추가로 보유하고 있다면 좋을 스킬셋이나 경험입니다
NeurIPS, ICML, ICLR, KDD, WWW, AAAI 등 AI top-tier 컨퍼런스학회에 논문을 게재하신 분
Kaggle 등 머신러닝 챌린지에서 입상하신 분
빅데이터에 대한 분석 경험이 있으신 분
분산 처리 시스템에 대한 성능 최적화 역량 및 경험
머신러닝을 서비스에 적용해본 경험이 있으신 분
초대형 규모의 딥러닝 모델을 학습시켜본 경험이 있으신 분
공유하기
http://www.naver-monthlyopening.com/#category-clova-ai-12
시계열 예측모델링 연구 ▼
이런 일을 맡고 있어요
네이버 및 라인의 비즈니스 지표 향상을 위해 AI를 적용하는 역할을 하고 있습니다.
최신 기계학습 방법론을 실제 비즈니스 문제에 적용하고 싶으신 마음이 있다면 현재 하고 있는 일이 무엇이든 도전해주세요.
실세계 데이터 분석, 기계학습 모델링, 모델성능의 실시간 평가 등 기계학습관련 전반적인 업무를 모두 경험하며 전문가로 성장할 수 있습니다.
역량있는 인재들이 함께 일하고 있으며 서로 성장에 도움을 주는 분위기를 구성하고 있습니다.
입사하게 되면 담당할 업무입니다
대규모 판매데이터 분석 및 피처추출
상품카탈로그매칭
SKU 단위 상품수요예측
업무를 수행하기 위해 필요한 자격 요건입니다
PyTorch, TensorFlow 등 딥러닝프레임워크 중 하나 이상 구현 역량
Hive, Presto, Spark 등 빅데이터 질의처리 프레임워크 지식 및 사용 경험
시계열 처리 알고리즘에 대한 기본지식
머신러닝, 딥러닝 모델에 대한 기본 지식
최신 딥러닝 기술을 이해하고 구현가능하신 분
Python, SQL 언어에 능숙하신 분
추가로 보유하고 있다면 좋을 스킬셋이나 경험입니다
NeurIPS, ICML, ICLR, KDD, WWW, AAAI 등 AI top-tier 컨퍼런스학회에 논문을 게재하신 분
Kaggle 등 머신러닝 챌린지에서 입상하신 분
사용자 빅데이터에 대한 분석 경험이 있으신 분
분산 처리 시스템에 대한 성능 최적화 역량 및 경험
머신러닝을 서비스에 적용해본 경험이 있으신 분
Computer vision, Natural Language Processing, Time-series 전문가
공유하기
http://www.naver-monthlyopening.com/#category-clova-ai-13
On-Device 딥러닝 인퍼런스 엔진 개발 ▼
이런 일을 맡고 있어요
Edge ML에서는 모바일을 비롯한 엣지 디바이스에서 딥러닝을 서비스하는 데에 필요한 전체 파이프라인을 다루고 있습니다.
엣지 디바이스향 인퍼런스 엔진의 고도화와 유저 친화적인 인터페이스 개발 등을 통해 이용자가 쉽고 빠르게 딥러닝을 서비스에 적용할 수 있도록 합니다.
현재 Edge ML에서 개발한 얼굴 인식 SDK는 LINE pay, 얼굴 인식 체크인 등 네이버 내 다양한 서비스에서 이용되고 있습니다.
입사하게 되면 담당할 업무입니다
모바일향 딥러닝 인퍼런스 엔진 고도화
업무를 수행하기 위해 필요한 자격 요건입니다
기본적인 비전 딥러닝 모델(CNN등)에 대한 이해
모바일용 딥러닝 인퍼런스 엔진(tflite, MNN 등)에 대한 깊은 이해
C++ 또는 Python 프로그래밍
추가로 보유하고 있다면 좋을 스킬셋이나 경험입니다
모바일이나 임베디드 환경에서 딥러닝 모델을 서비스 해본 경험
pytorch, tensorflow 등 다양한 딥러닝 프레임워크에 대한 깊은 이해
전통적인 비전 알고리즘에 관한 이해
공유하기
http://www.naver-monthlyopening.com/#category-clova-ai-14
On-Device 딥러닝 비전 SDK 개발 ▼
이런 일을 맡고 있어요
Edge ML에서는 모바일을 비롯한 엣지 디바이스에서 딥러닝을 서비스하는 데에 필요한 전체 파이프라인을 다루고 있습니다.
엣지 디바이스향 인퍼런스 엔진의 고도화와 유저 친화적인 인터페이스 개발 등을 통해 이용자가 쉽고 빠르게 딥러닝을 서비스에 적용할 수 있도록 합니다.
현재 Edge ML에서 개발한 얼굴 인식 SDK는 LINE pay, 얼굴 인식 체크인 등 네이버 내 다양한 서비스에서 이용되고 있습니다.
입사하게 되면 담당할 업무입니다
다양한 플랫폼(Android/iOS/Web/Python/Windows)에서 동작하는 SDK 개발
C++ 기반의 딥러닝 모델 인퍼런스 파이프라인 개선
업무를 수행하기 위해 필요한 자격 요건입니다
C/C++ 개발 및 아키텍처 경험
기본적인 비전 딥러닝 모델(CNN등)에 대한 이해
추가로 보유하고 있다면 좋을 스킬셋이나 경험입니다
모바일이나 임베디드 환경에서 딥러닝 모델을 서비스 해본 경험
오픈 소스 기여 경험
android, ios 앱 개발 경험
공유하기
http://www.naver-monthlyopening.com/#category-clova-ai-15
On-Device 딥러닝 NLP SDK 개발 ▼
이런 일을 맡고 있어요
Edge ML에서는 모바일을 비롯한 엣지 디바이스에서 딥러닝을 서비스하는 데에 필요한 전체 파이프라인을 다루고 있습니다.
엣지 디바이스향 인퍼런스 엔진의 고도화와 유저 친화적인 인터페이스 개발 등을 통해 이용자가 쉽고 빠르게 딥러닝을 서비스에 적용할 수 있도록 합니다.
현재 Edge ML에서는 새롭게 NLP를 이용한 텍스트 처리 프로젝트를 시작하고자 합니다.
입사하게 되면 담당할 업무입니다
MobileBERT를 비롯한 가벼운 NLP 모델을 이용한 on-device NLP SDK를 만들고 여러 프로젝트에 적용
업무를 수행하기 위해 필요한 자격 요건입니다
NLP 모델링 기술 경험
추가로 보유하고 있다면 좋을 스킬셋이나 경험입니다
C++
Android, iOS에서의 프로그래밍 경험
공유하기
http://www.naver-monthlyopening.com/#category-clova-ai-16
물류, 배송, 라스트마일 ML/Data Scientist ▼
이런 일을 맡고 있어요
네이버 그룹사의 물류/배송/SCM 도메인에 ML 도입을 하는 프로덕트 조직입니다.
일본의 No.1 푸드테크 서비스 데마에칸의 라스트마일 플랫폼을 개발하고 있으며, 배송, 풀필먼트, 물류의 전반적인 프로덕트를 직접 만들고 있으므로 여러 문제를 ML로 해결하며 성취감을 느낄 수 있습니다.
입사하게 되면 담당할 업무입니다
물류/배송 관련 데이터를 가공/정제하여 의미 있는 정보를 마이닝 합니다.
데이터를 기반으로 물류 도메인에 적용될 다양한 예측모델을 만듭니다.
업무를 수행하기 위해 필요한 자격 요건입니다
<DS>
- 데이터 정제 및 가공
- 빅데이터 분석 및 파이프라인 구축
- 데이터 가공 및 분산 처리 기술에 대한 이해
- 알고리즘, 데이터구조, OS, 데이터베이스 등 기본적인 전산 지식에 대한 이해
- 기본적인 SQL 및 Python, Jave 등을 활용한 프로그래밍 능력
- 다양한 빅데이터 프레임워크 사용 능력 (Hadoop, MR, Hive, Spark, etc.) 우대
<ML>
- 기본적인 학습 프레임워크 사용 능력 (PyTorch, Tensorflow, Keras 등)
- REST API에 대한 설계 및 개발 경험과 이해
- 수학 및 통계에 대한 깊이있는 배경지식
- 다양한 domain의 수요예측 관련 프로젝트 유 경험자 우대
추가로 보유하고 있다면 좋을 스킬셋이나 경험입니다
데이터에 대한 Insight가 있는 분 (이 분석을 왜 해야 하고 어떤 의미가 있는지 잘 전달할 수 있어야 함)
다양한 개발 언어나 프레임워크에 제약을 받지 않고, 필요한 것을 학습할 수 있는 분
문제를 끝까지 파고들어 해결한 경험이 있는 분 (개발 지구력)
팀 내에 개발 규칙이나 문화를 전파하고 리딩할 수 있는 분
공유하기
http://www.naver-monthlyopening.com/#category-clova-ai-17
전형 안내
전형 절차
지원서 접수 > 1차면접 > 2차면접 > 최종합격자 발표
네이버 조직/직무별 채용 전형 절차가 다르게 운영되고 있습니다. 따라서 채용 조직/직무에 따라 추가 전형이 포함될 수 있으며, 추가 전형으로는 전화면접, 코딩테스트, 사전 과제, 인성검사, 3차면접 등이 있을 수 있습니다.
각 전형별 상세 일정은 지원자별로 상이할 수 있으며, 합격자에게 개별 안내 후 진행됩니다.
채용 전형은 지원자 본인이 지원서 상에 기재한 희망 조직에서 우선적으로 검토하나, 보다 더 적합한 조직이 있는 경우 지원자 본인 동의 하에 조직이 변경될 수 있습니다.
지원 시 유의 사항
지원서 내용 중 허위사실이 있는 경우 합격이 취소될 수 있습니다.
국가유공자 및 장애인 등 취업보호대상자는 관계법령에 따라 우대합니다.
공고 마감 시점에는 지원자가 몰릴 수 있으니 가급적 마감 시점을 피해 최종 접수 부탁드립니다.
지원자 간 형평성을 위해 마감 후 추가 지원 접수는 불가한 점 유의 바랍니다.
기타 문의는 (네이버 커리어 홈페이지 > 지원문의 > 1:1 문의)를 통해 접수해 주시기 바랍니다.
