

.card {
    width: 1400px;
    height: 750px;
    perspective: 1000px;
  }
  
  .card-inner {
    width: 100%;
    height: 100%;
    position: relative;
    transform-style: preserve-3d;
    transition: transform 0.999s;
  }
  
  .card:hover .card-inner {
    transform: rotateY(180deg);
  }
  
  .card-front,
  .card-back {
    position: absolute;
    width: 100%;
    height: 100%;
    backface-visibility: hidden;
  }
  
  .card-front {
    background-color: #456aa1;
    color: #fff;
    display: flex;
    align-items: center;
    border: 10px solid #456aa1;
    border-radius: 10px;
    justify-content: center;
    font-size: 24px;
    transform: rotateY(0deg);
  }
  
  .card-back {
    background-color: #8e9626;
    color: #fff;
    display: flex;
    align-items: center;
    border: 10px solid #8e9626;
    border-radius: 10px;
    justify-content: center;
    font-size: 35px;
    transform: rotateY(180deg);
  }