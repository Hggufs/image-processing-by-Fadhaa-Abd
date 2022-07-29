# image-processing-by-Fadhaa-Abd
image processing 
clc;

clear all;

close all;

input_image=imread('cameraman.tif');

sobel_output = edge(input_image,'Sobel');

Roberts_output = edge(input_image,'Roberts');

Prewitt_output = edge(input_image,'Prewitt');

Laplacian_output = edge(input_image,'log');

Canny_output = edge(input_image,'Canny');

subplot(2,3,1);

imshow(input_image);

title('input image');

subplot(2,3,2);

imshow(sobel_output);

title('Sobel');

subplot(2,3,3);

imshow(Roberts_output);

title('Roberts');

subplot(2,3,4);

imshow(Prewitt_output);

title('Prewitt');

subplot(2,3,5);

imshow(Laplacian_output);

title('Laplacian of Gaussian(LOG)');

subplot(2,3,6);

imshow(Canny_output);

title('Canny');


