-- phpMyAdmin SQL Dump
-- version 4.5.1
-- http://www.phpmyadmin.net
--
-- Host: 127.0.0.1
-- Generation Time: Nov 29, 2017 at 09:49 PM
-- Server version: 10.1.16-MariaDB
-- PHP Version: 7.0.9

SET SQL_MODE = "NO_AUTO_VALUE_ON_ZERO";
SET time_zone = "+00:00";


/*!40101 SET @OLD_CHARACTER_SET_CLIENT=@@CHARACTER_SET_CLIENT */;
/*!40101 SET @OLD_CHARACTER_SET_RESULTS=@@CHARACTER_SET_RESULTS */;
/*!40101 SET @OLD_COLLATION_CONNECTION=@@COLLATION_CONNECTION */;
/*!40101 SET NAMES utf8mb4 */;

--
-- Database: `hotel`
--

-- --------------------------------------------------------

--
-- Table structure for table `admin`
--

CREATE TABLE `admin` (
  `admin_id` int(20) NOT NULL,
  `email` varchar(50) NOT NULL,
  `password` varchar(20) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=latin1;

-- --------------------------------------------------------

--
-- Table structure for table `booking`
--

CREATE TABLE `booking` (
  `booking_id` int(200) NOT NULL,
  `total_adult` int(50) NOT NULL,
  `total_children` int(50) NOT NULL,
  `checkin_date` date NOT NULL,
  `checkout_date` date NOT NULL,
  `special_requirement` text NOT NULL,
  `payment_status` varchar(50) NOT NULL,
  `total_amount` double DEFAULT NULL,
  `deposit` double NOT NULL,
  `booking_date` timestamp NOT NULL DEFAULT CURRENT_TIMESTAMP,
  `first_name` varchar(30) NOT NULL,
  `last_name` varchar(30) NOT NULL,
  `email` varchar(50) NOT NULL,
  `telephone_no` varchar(30) NOT NULL,
  `add_line1` varchar(100) NOT NULL,
  `add_line2` varchar(100) NOT NULL,
  `city` varchar(30) NOT NULL,
  `state` varchar(30) NOT NULL,
  `postcode` varchar(30) NOT NULL,
  `country` varchar(30) NOT NULL,
  `admin_id` int(10) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=latin1;

--
-- Dumping data for table `booking`
--

INSERT INTO `booking` (`booking_id`, `total_adult`, `total_children`, `checkin_date`, `checkout_date`, `special_requirement`, `payment_status`, `total_amount`, `deposit`, `booking_date`, `first_name`, `last_name`, `email`, `telephone_no`, `add_line1`, `add_line2`, `city`, `state`, `postcode`, `country`, `admin_id`) VALUES
(128, 1, 0, '2014-12-05', '2014-12-06', '', 'pending', 360, 54, '2014-12-05 03:49:58', 'Mohd Zulkarnain', 'Jaranee', 'mrzulkarnine@gmail.com', '0128951744', '307 Kpg Kanchong Jaya Gedong', 'None', 'Serian', 'Sarawak', '50600', 'Malaysia', 0),
(129, 1, 0, '2014-12-05', '2014-12-07', '', 'pending', 240, 36, '2014-12-05 04:53:27', 'Mohd Zulkarnain', 'Jaranee', 'mrzulkarnine@gmail.com', '0128951744', '307 Kpg Kanchong Jaya Gedong', 'None', 'Serian', 'Sarawak', '50600', 'Malaysia', 0),
(130, 1, 0, '2014-12-05', '2014-12-07', '', 'pending', 480, 72, '2014-12-05 04:58:13', 'Mohd Zulkarnain', 'Jaranee', 'mrzulkarnine@gmail.com', '0128951744', '307 Kpg Kanchong Jaya Gedong', 'None', 'Serian', 'Sarawak', '50600', 'Malaysia', 0),
(131, 2, 0, '2015-05-21', '2015-05-23', '', 'pending', 240, 36, '2015-05-20 19:16:14', 'Mohd Zulkarnain', 'Jaranee', 'mrzulkarnine@gmail.com', '0128951744', '307 Kpg Kanchong Jaya Gedong', '', 'Serian', 'Sarawak', '50600', 'Malaysia', 0),
(132, 2, 0, '2015-05-21', '2015-05-23', '', 'pending', 920, 138, '2015-05-20 19:18:52', 'Mohd Zulkarnain', 'Jaranee', 'mrzulkarnine@gmail.com', '0128951744', '307 Kpg Kanchong Jaya Gedong', '', 'Serian', 'Sarawak', '50600', 'Malaysia', 0),
(159, 4, 0, '2017-11-18', '2017-11-19', '', 'pending', 120, 18, '2017-11-18 08:14:28', '', '', '', '', '', '', '', '', '', '', 0),
(160, 1, 0, '2017-11-18', '2017-11-19', '', 'pending', 120, 18, '2017-11-18 08:22:19', '', '', 'rr@gmail.com', '', '', '', '', '', '560070', '', 0),
(161, 2, 0, '2017-11-18', '2017-11-19', '', 'confirmed', 200, 30, '2017-11-18 09:13:03', '', '', 'rr@gmail.com', '', '', '', '', '', '560070', '', 0),
(162, 4, 0, '2017-11-19', '2017-11-19', '', 'pending', 0, 0, '2017-11-18 09:48:38', '', '', '', '', '', '', '', '', '', '', 0),
(163, 3, 0, '2017-11-18', '2017-11-19', '', 'pending', 200, 30, '2017-11-18 09:49:06', '', '', '', '', '', '', '', '', '', '', 0),
(164, 4, 0, '2017-11-18', '2017-11-19', '', 'pending', 360, 54, '2017-11-18 09:54:43', '', '', 'rr@gmail.com', '', '', '', '', '', '560070', '', 0),
(165, 2, 0, '1970-01-01', '1970-01-01', '', 'pending', 0, 0, '2017-11-18 14:09:33', '', '', '', '', '', '', '', '', '', '', 0),
(166, 2, 0, '1970-01-01', '1970-01-01', '', 'pending', 0, 0, '2017-11-18 14:11:50', '', '', '', '', '', '', '', '', '', '', 0),
(167, 3, 0, '1970-01-01', '1970-01-01', '', 'pending', 0, 0, '2017-11-18 14:13:00', '', '', '', '', '', '', '', '', '', '', 0),
(168, 3, 0, '1970-01-01', '1970-01-01', '', 'pending', 0, 0, '2017-11-18 14:13:01', '', '', '', '', '', '', '', '', '', '', 0),
(169, 3, 0, '1970-01-01', '1970-01-01', '', 'pending', 0, 0, '2017-11-18 14:19:39', '', '', '', '', '', '', '', '', '', '', 0),
(170, 3, 0, '1970-01-01', '1970-01-01', '', 'pending', 0, 0, '2017-11-18 14:19:40', '', '', '', '', '', '', '', '', '', '', 0),
(171, 2, 0, '1970-01-01', '1970-01-01', '', 'pending', 0, 0, '2017-11-18 14:22:48', '', '', '', '', '', '', '', '', '', '', 0),
(172, 1, 0, '1970-01-01', '1970-01-01', '', 'pending', 120, 18, '2017-11-18 14:26:08', '', '', '', '', '', '', '', '', '', '', 0),
(173, 2, 0, '1970-01-01', '1970-01-01', '', 'pending', 120, 18, '2017-11-18 14:29:40', '', '', '', '', '', '', '', '', '', '', 0),
(174, 2, 0, '1970-01-01', '1970-01-01', '', 'pending', 0, 0, '2017-11-18 14:30:38', '', '', '', '', '', '', '', '', '', '', 0),
(175, 3, 0, '1970-01-01', '1970-01-01', '', 'pending', 0, 0, '2017-11-18 14:31:13', '', '', '', '', '', '', '', '', '', '', 0),
(176, 3, 0, '1970-01-01', '1970-01-01', '', 'pending', 120, 18, '2017-11-18 14:31:43', '', '', '', '', '', '', '', '', '', '', 0),
(177, 3, 0, '2017-11-18', '2017-11-18', '', 'pending', 0, 0, '2017-11-18 14:48:39', '', '', '', '', '', '', '', '', '', '', 0),
(178, 2, 0, '2017-11-18', '2017-11-18', '', 'pending', 0, 0, '2017-11-18 14:49:22', '', '', '', '', '', '', '', '', '', '', 0),
(179, 3, 0, '2017-11-18', '2017-11-19', '', 'pending', 120, 18, '2017-11-18 14:50:28', '', '', '', '', '', '', '', '', '', '', 0),
(180, 3, 0, '2017-11-18', '2017-11-19', '', 'pending', 360, 54, '2017-11-18 14:51:23', '', '', '', '', '', '', '', '', '', '', 0),
(181, 3, 0, '2017-11-19', '2017-11-20', '', 'pending', 120, 18, '2017-11-18 14:55:02', '', '', '', '', '', '', '', '', '', '', 0),
(182, 3, 0, '2017-11-19', '2017-11-20', '', 'pending', 360, 54, '2017-11-18 14:55:15', '', '', '', '', '', '', '', '', '', '', 0),
(183, 3, 0, '2017-11-19', '2017-11-20', '', 'pending', 480, 72, '2017-11-18 14:57:38', '', '', '', '', '', '', '', '', '', '', 0),
(184, 2, 0, '1970-01-01', '1970-01-01', '', 'pending', 120, 18, '2017-11-18 14:58:22', '', '', '', '', '', '', '', '', '', '', 0),
(185, 2, 0, '2017-11-20', '2017-11-21', '', 'pending', 240, 36, '2017-11-18 16:44:02', '', '', '', '', '', '', '', '', '', '', 0),
(186, 2, 0, '1970-01-01', '1970-01-01', '', 'pending', 120, 18, '2017-11-18 16:45:09', '', '', 'rr@gmail.com', '', '', '', '', '', '560070', '', 0),
(187, 2, 0, '2017-11-18', '2017-11-19', '', 'pending', 1000, 150, '2017-11-18 18:02:10', '', '', 'rr@gmail.com', '', '', '', '', '', '560070', '', 0),
(188, 2, 0, '2017-11-18', '2017-11-19', '', 'pending', 1500, 225, '2017-11-18 18:06:00', '', '', 'rr@gmail.com', '', '', '', '', '', '560070', '', 1),
(189, 1, 0, '2017-11-21', '2017-11-23', '', 'pending', 240, 36, '2017-11-18 18:45:53', '', '', '', '', '', '', '', '', '', '', 2),
(190, 2, 0, '2017-11-19', '2017-11-20', '', 'pending', 500, 75, '2017-11-18 19:03:37', 'xcv', 'cxv', 'rr@gmail.com', '1234567830', '', '', '', '', '560070', '', 0),
(191, 2, 0, '2017-11-19', '2017-11-20', '', 'pending', 240, 36, '2017-11-18 19:06:40', 'xcv', 'cxv', 'rr@gmail.com', '1234567830', '', '', '', '', '560070', '', 2),
(192, 3, 0, '1970-01-01', '1970-01-01', '', 'pending', 100, 15, '2017-11-18 19:30:16', '', '', 'rr@gmail.com', '', '', '', '', '', '560070', '', 1),
(193, 1, 0, '2017-11-19', '2017-11-19', '', 'confirmed', 0, 0, '2017-11-19 09:47:35', '', '', 'rr@gmail.com', '', '', '', '', '', '', '', 1),
(194, 1, 0, '2017-11-19', '2017-11-20', '', 'pending', 120, 18, '2017-11-19 11:16:50', '', '', '', '', '', '', '', '', '', '', 0),
(195, 1, 0, '2017-11-21', '2017-11-23', '', 'pending', 240, 36, '2017-11-19 15:17:52', '', '', '', '', '', '', '', '', '', '', 0),
(196, 1, 0, '2017-11-21', '2017-11-23', '', 'pending', 480, 72, '2017-11-19 15:18:23', '', '', '', '', '', '', '', '', '', '', 0),
(197, 2, 0, '2017-11-22', '2017-11-24', '', 'pending', 720, 108, '2017-11-19 15:18:48', '', '', '', '', '', '', '', '', '', '', 0),
(198, 1, 0, '2017-11-26', '2017-11-29', '', 'pending', 360, 54, '2017-11-19 15:22:34', '', '', '', '', '', '', '', '', '', '', 0),
(199, 2, 0, '2017-11-20', '2017-11-23', '', 'pending', 360, 54, '2017-11-19 15:23:15', '', '', '', '', '', '', '', '', '', '', 0),
(200, 1, 0, '2017-11-19', '2017-11-23', '', 'pending', 400, 60, '2017-11-19 15:24:16', '', '', '', '', '', '', '', '', '', '', 0),
(201, 1, 0, '2017-11-19', '2017-11-21', '', 'pending', 400, 60, '2017-11-19 15:26:12', '', '', '', '', '', '', '', '', '', '', 0),
(202, 1, 0, '2017-11-20', '2017-11-21', '', 'pending', 120, 18, '2017-11-19 15:28:41', '', '', '', '', '', '', '', '', '', '', 0),
(203, 1, 0, '2017-11-19', '2017-11-21', '', 'pending', 480, 72, '2017-11-19 15:39:18', 'xcv', 'cxv', 'rr@gmail.com', '1234567830', '', '', '', '', '560070', '', 2),
(204, 1, 0, '2017-11-20', '2017-11-21', '', 'pending', 100, 15, '2017-11-19 17:51:27', 'xcv', 'cxv', 'rr@gmail.com', '1234567830', '', '', '', '', '560070', '', 0),
(205, 1, 0, '2017-11-28', '2017-11-30', '', 'pending', 240, 36, '2017-11-27 16:15:23', 'xcv', 'cxv', 'rr@gmail.com', '1234567830', '', '', '', '', '560070', '', 0);

-- --------------------------------------------------------

--
-- Table structure for table `flight`
--

CREATE TABLE `flight` (
  `flight_id` int(255) NOT NULL,
  `total_seats` int(255) NOT NULL,
  `occupancy` int(255) DEFAULT NULL,
  `size` varchar(30) DEFAULT NULL,
  `view` varchar(30) DEFAULT NULL,
  `flight_name` varchar(50) NOT NULL,
  `flight_from` varchar(150) NOT NULL,
  `flight_to` varchar(150) NOT NULL,
  `descriptions` text,
  `rate` double NOT NULL,
  `imgpath` varchar(100) NOT NULL,
  `admin_id` int(10) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=latin1;

--
-- Dumping data for table `flight`
--

INSERT INTO `flight` (`flight_id`, `total_seats`, `occupancy`, `size`, `view`, `flight_name`, `flight_from`, `flight_to`, `descriptions`, `rate`, `imgpath`, `admin_id`) VALUES
(1, 10, 1, '10 sqft', 'city', 'Air India', 'Delhi', 'Mumbai', 'Neque porro quisquam est qui dolorem ipsum quia dolor', 150, 'img/air_india.jpg', 0),
(2, 5, 1, '10 sqft', 'city', 'Indigo', 'Bengaluru', 'Dubai', 'Neque porro quisquam est qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit', 100, 'img/indigo.jpg', 1),
(3, 10, 1, '20 sqft', 'City', 'British Airways', 'Chicago', 'London', 'Suitable for honeymoon', 120, 'img/british.jpg', 2),
(5, 150, 0, '', '', 'Singapore Airlines', 'testfrom', 'testto', 'Economy Premium at its best', 250, 'img/1200px-Singapore_Airlines_Logo.svg.png', 1);

-- --------------------------------------------------------

--
-- Table structure for table `flightbook`
--

CREATE TABLE `flightbook` (
  `booking_id` int(11) NOT NULL,
  `flight_id` int(11) NOT NULL,
  `totalflightbook` int(11) NOT NULL,
  `id` int(11) NOT NULL,
  `admin_id` int(10) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=latin1;

--
-- Dumping data for table `flightbook`
--

INSERT INTO `flightbook` (`booking_id`, `flight_id`, `totalflightbook`, `id`, `admin_id`) VALUES
(193, 1, 2, 1, 1);

-- --------------------------------------------------------

--
-- Table structure for table `flight_admin`
--

CREATE TABLE `flight_admin` (
  `id` int(11) NOT NULL,
  `username` varchar(300) NOT NULL,
  `password` varchar(300) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=latin1;

--
-- Dumping data for table `flight_admin`
--

INSERT INTO `flight_admin` (`id`, `username`, `password`) VALUES
(1, 'flt_admin', 'flt_admin'),
(2, 'gh', 'gh'),
(3, 'rt', 'rt');

-- --------------------------------------------------------

--
-- Table structure for table `flight_booking`
--

CREATE TABLE `flight_booking` (
  `booking_id` int(200) NOT NULL,
  `total_adult` int(50) NOT NULL,
  `total_children` int(50) NOT NULL,
  `checkin_date` date NOT NULL,
  `checkout_date` date NOT NULL,
  `flight_from` varchar(150) NOT NULL,
  `flight_to` varchar(150) NOT NULL,
  `special_requirement` text NOT NULL,
  `payment_status` varchar(50) NOT NULL,
  `total_amount` double DEFAULT NULL,
  `deposit` double NOT NULL,
  `booking_date` timestamp NOT NULL DEFAULT CURRENT_TIMESTAMP,
  `first_name` varchar(30) NOT NULL,
  `last_name` varchar(30) NOT NULL,
  `email` varchar(50) NOT NULL,
  `telephone_no` varchar(30) NOT NULL,
  `add_line1` varchar(100) NOT NULL,
  `add_line2` varchar(100) NOT NULL,
  `city` varchar(30) NOT NULL,
  `state` varchar(30) NOT NULL,
  `postcode` varchar(30) NOT NULL,
  `country` varchar(30) NOT NULL,
  `admin_id` int(10) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=latin1;

--
-- Dumping data for table `flight_booking`
--

INSERT INTO `flight_booking` (`booking_id`, `total_adult`, `total_children`, `checkin_date`, `checkout_date`, `flight_from`, `flight_to`, `special_requirement`, `payment_status`, `total_amount`, `deposit`, `booking_date`, `first_name`, `last_name`, `email`, `telephone_no`, `add_line1`, `add_line2`, `city`, `state`, `postcode`, `country`, `admin_id`) VALUES
(193, 2, 0, '2017-11-19', '2017-11-19', '', '', '', 'confirmed', 120, 18, '2017-11-18 19:45:28', '', '', 'rr@gmail.com', '', '', '', '', '', '560070', '', 2),
(194, 2, 0, '1970-01-01', '1970-01-01', '', '', '', 'confirmed', 120, 18, '2017-11-19 09:43:19', '', '', '', '', '', '', '', '', '', '', 0),
(195, 1, 0, '1970-01-01', '1970-01-01', '', '', '', 'pending', 100, 15, '2017-11-19 10:18:26', '', '', '', '', '', '', '', '', '', '', 1),
(196, 2, 0, '0000-00-00', '0000-00-00', '', '', '', 'pending', 120, 18, '2017-11-19 10:29:38', '', '', '', '', '', '', '', '', '', '', 0),
(197, 1, 0, '0000-00-00', '0000-00-00', '', '', '', 'pending', 120, 18, '2017-11-19 10:30:02', '', '', '', '', '', '', '', '', '', '', 0),
(198, 1, 0, '0000-00-00', '0000-00-00', '', '', '', 'pending', 120, 18, '2017-11-19 10:31:26', '', '', '', '', '', '', '', '', '', '', 0),
(199, 2, 0, '0000-00-00', '0000-00-00', '', '', '', 'pending', 120, 18, '2017-11-19 10:40:02', '', '', '', '', '', '', '', '', '', '', 0),
(200, 2, 0, '0000-00-00', '0000-00-00', 'Delhi', 'Mumbai', '', 'pending', 120, 18, '2017-11-19 12:38:25', '', '', '', '', '', '', '', '', '', '', 0),
(201, 2, 0, '0000-00-00', '0000-00-00', 'Bengalore', 'Dubai', '', 'pending', 100, 15, '2017-11-19 12:42:51', '', '', '', '', '', '', '', '', '', '', 1),
(202, 1, 0, '2017-11-19', '2017-11-21', '', '', '', 'pending', 0, 0, '2017-11-19 17:50:49', '', '', 'rr@gmail.com', '', '', '', '', '', '560070', '', 0),
(203, 1, 0, '2017-11-20', '2017-11-21', '', '', '', 'pending', 100, 15, '2017-11-19 17:51:43', '', '', 'rr@gmail.com', '', '', '', '', '', '560070', '', 0),
(204, 2, 0, '2017-11-20', '2017-11-21', '', '', '', 'pending', 100, 15, '2017-11-19 17:56:48', '', '', 'rr@gmail.com', '', '', '', '', '', '560070', '', 0),
(205, 1, 0, '0000-00-00', '0000-00-00', 'Delhi', 'Mumbai', '', 'pending', 120, 18, '2017-11-19 18:02:05', '', '', 'rr@gmail.com', '', '', '', '', '', '560070', '', 0),
(206, 2, 0, '0000-00-00', '0000-00-00', 'Delhi', 'Mumbai', '', 'pending', 0, 0, '2017-11-19 18:05:35', '', '', 'rr@gmail.com', '', '', '', '', '', '560070', '', 0),
(207, 1, 0, '0000-00-00', '0000-00-00', 'Delhi', 'Mumbai', '', 'pending', 0, 0, '2017-11-19 18:07:52', '', '', 'rr@gmail.com', '', '', '', '', '', '560070', '', 0),
(208, 2, 0, '0000-00-00', '0000-00-00', 'Delhi', 'Mumbai', '', 'pending', 480, 0, '2017-11-19 18:24:36', '', '', 'rr@gmail.com', '', '', '', '', '', '560070', '', 0),
(209, 1, 0, '0000-00-00', '0000-00-00', 'Delhi', 'Mumbai', '', 'pending', 120, 0, '2017-11-19 18:28:06', '', '', 'rr@gmail.com', '', '', '', '', '', '560070', '', 0),
(210, 1, 0, '0000-00-00', '0000-00-00', 'Delhi', 'Mumbai', '', 'pending', 240, 0, '2017-11-19 18:28:26', '', '', 'rr@gmail.com', '', '', '', '', '', '560070', '', 0),
(211, 2, 0, '0000-00-00', '0000-00-00', 'Delhi', 'Mumbai', '', 'pending', 480, 72, '2017-11-19 18:35:32', '', '', 'rr@gmail.com', '', '', '', '', '', '560070', '', 0),
(212, 0, 0, '0000-00-00', '0000-00-00', 'Delhi', 'Mumbai', '', 'pending', 0, 0, '2017-11-19 18:36:05', '', '', 'rr@gmail.com', '', '', '', '', '', '560070', '', 0),
(213, 2, 0, '0000-00-00', '0000-00-00', 'Delhi', 'Mumbai', '', 'pending', 480, 72, '2017-11-19 18:36:19', '', '', 'rr@gmail.com', '', '', '', '', '', '560070', '', 0),
(214, 3, 0, '0000-00-00', '0000-00-00', 'Delhi', 'Mumbai', '', 'pending', 360, 54, '2017-11-19 18:37:13', '', '', 'rr@gmail.com', '', '', '', '', '', '560070', '', 0),
(215, 1, 0, '0000-00-00', '0000-00-00', 'Delhi', 'Mumbai', '', 'pending', 480, 72, '2017-11-19 18:53:36', '', '', 'rr@gmail.com', '', '', '', '', '', '560070', '', 0);

-- --------------------------------------------------------

--
-- Table structure for table `hotel_admin`
--

CREATE TABLE `hotel_admin` (
  `id` int(11) NOT NULL,
  `username` varchar(300) NOT NULL,
  `password` varchar(300) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=latin1;

--
-- Dumping data for table `hotel_admin`
--

INSERT INTO `hotel_admin` (`id`, `username`, `password`) VALUES
(1, 'hotl_admin', 'hotl_admin'),
(2, 'tt', 'tt'),
(3, 'rt', 'rt');

-- --------------------------------------------------------

--
-- Table structure for table `register`
--

CREATE TABLE `register` (
  `register_id` int(200) NOT NULL,
  `first_name` varchar(30) NOT NULL,
  `last_name` varchar(30) NOT NULL,
  `email` varchar(50) NOT NULL,
  `telephone_no` varchar(30) NOT NULL,
  `add_line1` varchar(100) NOT NULL,
  `add_line2` varchar(100) NOT NULL,
  `postcode` varchar(30) NOT NULL,
  `password` varchar(30) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=latin1;

--
-- Dumping data for table `register`
--

INSERT INTO `register` (`register_id`, `first_name`, `last_name`, `email`, `telephone_no`, `add_line1`, `add_line2`, `postcode`, `password`) VALUES
(1, 'xcv', 'cxv', 'rr@gmail.com', '1234567830', 'xcv', 'zdfg', '560070', 'ravi');

-- --------------------------------------------------------

--
-- Table structure for table `room`
--

CREATE TABLE `room` (
  `room_id` int(255) NOT NULL,
  `total_room` int(255) NOT NULL,
  `occupancy` int(255) DEFAULT NULL,
  `size` varchar(30) DEFAULT NULL,
  `view` varchar(30) DEFAULT NULL,
  `room_name` varchar(50) NOT NULL,
  `descriptions` text,
  `rate` int(150) NOT NULL,
  `imgpath` varchar(100) NOT NULL,
  `admin_id` int(11) NOT NULL,
  `location` varchar(150) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=latin1;

--
-- Dumping data for table `room`
--

INSERT INTO `room` (`room_id`, `total_room`, `occupancy`, `size`, `view`, `room_name`, `descriptions`, `rate`, `imgpath`, `admin_id`, `location`) VALUES
(2, 5, 2, '10 sqft', 'city', 'Single Room', 'Neque porro ', 150, 'img/room3.png', 1, 'bengaluru'),
(3, 20, 2, '250', 'city', 'Delux', 'vadkraj', 367, 'img/room2.jpg', 2, 'mumbai');

-- --------------------------------------------------------

--
-- Table structure for table `roombook`
--

CREATE TABLE `roombook` (
  `booking_id` int(11) NOT NULL,
  `room_id` int(11) NOT NULL,
  `totalroombook` int(11) NOT NULL,
  `id` int(11) NOT NULL,
  `admin_id` int(10) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=latin1;

--
-- Dumping data for table `roombook`
--

INSERT INTO `roombook` (`booking_id`, `room_id`, `totalroombook`, `id`, `admin_id`) VALUES
(128, 3, 3, 69, 0),
(129, 1, 1, 70, 0),
(130, 1, 1, 71, 0),
(131, 1, 1, 72, 0),
(132, 1, 2, 73, 0),
(0, 1, 1, 86, 0),
(160, 1, 1, 87, 0),
(161, 2, 2, 88, 0),
(162, 2, 2, 89, 0),
(163, 2, 2, 90, 0),
(164, 3, 3, 91, 0),
(177, 3, 3, 92, 0),
(178, 3, 1, 93, 0),
(179, 3, 1, 94, 0),
(180, 3, 2, 95, 0),
(181, 1, 1, 96, 0),
(182, 3, 2, 97, 0),
(183, 1, 1, 98, 0),
(185, 1, 1, 99, 0),
(187, 4, 2, 100, 1),
(188, 4, 1, 101, 1),
(189, 3, 1, 102, 2),
(190, 4, 1, 103, 1),
(191, 3, 2, 104, 2),
(193, 4, 1, 105, 1),
(194, 1, 1, 106, 0),
(195, 1, 1, 107, 0),
(196, 1, 1, 108, 0),
(197, 1, 1, 109, 0),
(198, 1, 1, 110, 0),
(199, 1, 1, 111, 0),
(200, 2, 1, 112, 0),
(201, 2, 2, 113, 0),
(202, 1, 1, 114, 0),
(203, 3, 2, 115, 2),
(204, 2, 1, 116, 0),
(205, 1, 1, 117, 0);

-- --------------------------------------------------------

--
-- Table structure for table `user`
--

CREATE TABLE `user` (
  `id` int(11) NOT NULL,
  `username` varchar(300) NOT NULL,
  `password` varchar(300) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=latin1;

--
-- Dumping data for table `user`
--

INSERT INTO `user` (`id`, `username`, `password`) VALUES
(1, 'demo', 'demo');

--
-- Indexes for dumped tables
--

--
-- Indexes for table `admin`
--
ALTER TABLE `admin`
  ADD PRIMARY KEY (`admin_id`);

--
-- Indexes for table `booking`
--
ALTER TABLE `booking`
  ADD PRIMARY KEY (`booking_id`);

--
-- Indexes for table `flight`
--
ALTER TABLE `flight`
  ADD PRIMARY KEY (`flight_id`);

--
-- Indexes for table `flightbook`
--
ALTER TABLE `flightbook`
  ADD PRIMARY KEY (`booking_id`);

--
-- Indexes for table `flight_admin`
--
ALTER TABLE `flight_admin`
  ADD PRIMARY KEY (`id`);

--
-- Indexes for table `flight_booking`
--
ALTER TABLE `flight_booking`
  ADD PRIMARY KEY (`booking_id`);

--
-- Indexes for table `hotel_admin`
--
ALTER TABLE `hotel_admin`
  ADD PRIMARY KEY (`id`);

--
-- Indexes for table `register`
--
ALTER TABLE `register`
  ADD PRIMARY KEY (`register_id`);

--
-- Indexes for table `room`
--
ALTER TABLE `room`
  ADD PRIMARY KEY (`room_id`);

--
-- Indexes for table `roombook`
--
ALTER TABLE `roombook`
  ADD PRIMARY KEY (`id`);

--
-- Indexes for table `user`
--
ALTER TABLE `user`
  ADD PRIMARY KEY (`id`);

--
-- AUTO_INCREMENT for dumped tables
--

--
-- AUTO_INCREMENT for table `admin`
--
ALTER TABLE `admin`
  MODIFY `admin_id` int(20) NOT NULL AUTO_INCREMENT;
--
-- AUTO_INCREMENT for table `booking`
--
ALTER TABLE `booking`
  MODIFY `booking_id` int(200) NOT NULL AUTO_INCREMENT, AUTO_INCREMENT=206;
--
-- AUTO_INCREMENT for table `flight`
--
ALTER TABLE `flight`
  MODIFY `flight_id` int(255) NOT NULL AUTO_INCREMENT, AUTO_INCREMENT=12;
--
-- AUTO_INCREMENT for table `flight_admin`
--
ALTER TABLE `flight_admin`
  MODIFY `id` int(11) NOT NULL AUTO_INCREMENT, AUTO_INCREMENT=4;
--
-- AUTO_INCREMENT for table `flight_booking`
--
ALTER TABLE `flight_booking`
  MODIFY `booking_id` int(200) NOT NULL AUTO_INCREMENT, AUTO_INCREMENT=216;
--
-- AUTO_INCREMENT for table `hotel_admin`
--
ALTER TABLE `hotel_admin`
  MODIFY `id` int(11) NOT NULL AUTO_INCREMENT, AUTO_INCREMENT=4;
--
-- AUTO_INCREMENT for table `register`
--
ALTER TABLE `register`
  MODIFY `register_id` int(200) NOT NULL AUTO_INCREMENT, AUTO_INCREMENT=8;
--
-- AUTO_INCREMENT for table `room`
--
ALTER TABLE `room`
  MODIFY `room_id` int(255) NOT NULL AUTO_INCREMENT, AUTO_INCREMENT=10;
--
-- AUTO_INCREMENT for table `roombook`
--
ALTER TABLE `roombook`
  MODIFY `id` int(11) NOT NULL AUTO_INCREMENT, AUTO_INCREMENT=118;
--
-- AUTO_INCREMENT for table `user`
--
ALTER TABLE `user`
  MODIFY `id` int(11) NOT NULL AUTO_INCREMENT, AUTO_INCREMENT=2;
/*!40101 SET CHARACTER_SET_CLIENT=@OLD_CHARACTER_SET_CLIENT */;
/*!40101 SET CHARACTER_SET_RESULTS=@OLD_CHARACTER_SET_RESULTS */;
/*!40101 SET COLLATION_CONNECTION=@OLD_COLLATION_CONNECTION */;
