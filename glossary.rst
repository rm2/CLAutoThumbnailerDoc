.. default-role:: filename

==========
 Glossary
==========

.. glossary::
   :sorted:

   aspect ratio
      The width divided by the height of an image. See
      http://en.wikipedia.org/wiki/Aspect_ratio_(image) for more
      information.

      `DVD Pictures
      <http://www.highdefinitionblog.com/Pages/DVDPictures.htm>` has a
      number of nice examples explaining the issues involved with
      terminology such as Fullscreen, Widescreen, and HD aspect ratios.

   Command File
      A text file that contains entries that specify the options to use
      while processing a video file along with the relative path to that
      file. See :doc:`ref-commandfile` for more information.

   Column Priority Layout
      A thumbnail page layout mode in which the exact number of columns
      is set while the number of rows is automatically determined to fit
      in the desired page size. Only used for videos that have an
      :term:`aspect ratio` that is smaller than 1.36 for an
      :term:`Overview thumbnail page`, or 1.44 for :term:`Detail
      thumbnail pages`.

   Row Priority Layout
      A thumbnail page layout mode in which the exact number of rows is
      set while the number of columns is automatically determined to fit
      in the desired page size. Used for videos that have an
      :term:`aspect ratio` that is greater than or equal to 1.36 for an
      :term:`Overview thumbnail page`, or 1.44 for :term:`Detail
      thumbnail pages`.

   Actual Layout
      Thumbnail pages will have exactly the number of columns and rows
      specified. No consideration is taken of the amount of space that
      might be wasted.

   Overview thumbnail page
      A single thumbnail page for an entire video file, typically with a
      larger number of rows and columns (in the range of 9-12) than
      :term:`Detail thumbnail pages` . The Overview page can be turned
      off with the :option:`-k` option.

      .. figure:: images/his_girl_friday_512kb_nocredits_overview.jpg
         :scale: 50%
         :align: center
         :alt: Example Overview Thumbnail Page
         :target: _images/his_girl_friday_512kb_nocredits_overview.jpg

         Example Overview Thumbnail Page


   Detail thumbnail pages
      Thumbnail pages that contain thumbnails that are generated a fixed
      amount of time from each other (like every minute). Detail pages
      will be made as needed until the entire video has been
      thumbnailed. Typically with a smaller number of rows and columns
      (in the range of 3-6) than a :term:`Overview thumbnail
      page`. Detail page generation can be turned off by using the
      :option:`-i` option.

      .. figure:: images/his_girl_friday_512kb_page0001_00_00_05.jpg
         :scale: 50%
         :align: center
         :alt: Example Detail Thumbnail Page
         :target: _images/his_girl_friday_512kb_page0001_00_00_05.jpg

         Example Detail Thumbnail Page

   VOB
      The file extension used for video files on DVDs. These files are
      actually in the MPEG2 format. VOB title sets are named
      `VTS_tt_n.VOB` where ``tt`` is the title number and ``n`` is the
      number of the file within that title. |CLATN| can treat an
      unencrypted VOB title set as a single long video by specifying
      `VTS_tt_*.VOB` as the filename (where ``tt`` should be replaced
      with the number of the title you wish to thumbnail).


   codec
      The method by which a video has been turned into a viewable
      file. Requires a matching decoder to view. See
      http://en.wikipedia.org/wiki/Video_codec and
      http://en.wikipedia.org/wiki/List_of_codecs for more
      information.


..
   Local Variables:
   coding: utf-8
   mode: rst
   End:
