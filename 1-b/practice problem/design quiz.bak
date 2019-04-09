;; The first three lines of this file were inserted by DrRacket. They record metadata
;; about the language level of this file in a form that our tools can easily process.
#reader(lib "htdp-beginner-reader.ss" "lang")((modname |design quiz|) (read-case-sensitive #t) (teachpacks ()) (htdp-settings #(#t constructor repeating-decimal #f #t none #f () #f)))
(require 2htdp/image)

;; Image, Image -> Boolean    ;signture
;; given 2 Images, return true if the first frame area > the second frame area     ;prupose
(check-expect (Image-compare? (rectangle 20 20 "solid" "red") (rectangle 20 10 "solid" "red")) true)
(check-expect (Image-compare? (rectangle 10 10 "solid" "red") (rectangle 20 10 "solid" "red")) false)
(check-expect (Image-compare? (rectangle 20 10 "solid" "red") (rectangle 20 10 "solid" "red")) false)

;(define (Image-compare? img1 img2) false)     ;stub

;(define (Image-compare? img1 img2)         ;template
;  ((.....img1) (......img2)))

(define (Image-compare? img1 img2)
  (> (* (image-width img1) (image-height img1))
     (* (image-width img2) (image-height img2))))